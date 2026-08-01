---
name: Navigate a Polymath robot with GPS waypoints
description: Authenticate, confirm the robot is healthy, send a set of GPS waypoints, and monitor navigation feedback until the goal completes.
api: openapi/polymath-synapse-v2-openapi-original.json
operations: [get_health, get_device_uuid, gps_waypoints, polymath_feedback]
---

# Navigate a Polymath robot with GPS waypoints

Use this to drive a real or simulated Polymath-powered vehicle to a sequence of GPS points.

## Auth
Obtain a bearer token via the OAuth 2.0 client-credentials flow: POST `client_id`, `client_secret`, `audience=https://api.polymathrobotics.dev/`, `grant_type=client_credentials` to `https://polyglot.polymathrobotics.dev/oauth/token`. Send `Authorization: Bearer <access_token>` on every call. All paths are routed through `https://polyglot.polymathrobotics.dev/api/synapse/{DEVICE_ID}/v2`.

## Steps
1. `get_health` (GET /v2/health) - confirm the robot/gateway is up before commanding motion.
2. `get_device_uuid` (GET /v2/uuid) - confirm you are addressing the intended device.
3. `gps_waypoints` (POST /v2/gps-waypoints) - send the ordered waypoints; each point carries `lat`, `lon`, `yaw`.
4. `polymath_feedback` (GET /v2/polymath-feedback) - poll combined autonomy/navigation/vehicle feedback until the navigation goal reports complete.

## Rules
- There is no idempotency-key contract; do not blindly retry a POST after a timeout - re-read feedback first (see conventions/polymath-conventions.yml).
- 401 means refresh the token; 403 means a teleop control lease is required or held elsewhere (see the teleop skill).
- Errors return `{ status: "error", message, error.details }` (see errors/polymath-problem-types.yml).
