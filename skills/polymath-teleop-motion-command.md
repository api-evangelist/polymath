---
name: Take exclusive teleop control and send a motion command
description: Acquire the exclusive teleoperation control lease, verify it is held, issue a motion command, then release the lease.
api: openapi/polymath-synapse-v2-openapi-original.json
operations: [acquire_lease, get_lease_status, get_nav_cmds, nav_cmd, release_lease]
---

# Take exclusive teleop control and send a motion command

Control/write operations require an exclusive lease. This skill acquires it, acts, and releases it cleanly.

## Auth
Bearer token via OAuth 2.0 client-credentials (see the authentication guide). Send `Authorization: Bearer <token>` on every call.

## Steps
1. `acquire_lease` (POST /v2/teleop-control/acquire) - obtain the exclusive control lease. If it returns 403 the lease is held by another user; wait or request a transfer.
2. `get_lease_status` (GET /v2/teleop-control/status) - confirm you hold the lease before commanding motion.
3. `get_nav_cmds` (GET /v2/motion-commands) - list the available motion commands and their parameters.
4. `nav_cmd` (POST /v2/motion-command) - send the chosen motion command to change the robot's state.
5. `release_lease` (POST /v2/teleop-control/release) - always release the lease when done so other operators are not blocked.

## Rules
- Renew the lease with `renew_lease` (POST /v2/teleop-control/renew) before it expires during long sessions.
- Any control call without a held lease returns 403 (see errors/polymath-problem-types.yml).
- Prefer `transfer_lease` over forcing a takeover when another operator holds control.
