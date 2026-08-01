---
name: Set a reference target and read autonomy feedback
description: Register a reference location or object, list all reference targets, and read the combined autonomy/navigation/vehicle feedback.
api: openapi/polymath-synapse-v2-openapi-original.json
operations: [set_reference_targets, set_reference_target_current_location, reference_targets, polymath_feedback]
---

# Set a reference target and read autonomy feedback

Reference targets anchor named locations or objects in the robot's world frame for later navigation.

## Auth
Bearer token via OAuth 2.0 client-credentials; send `Authorization: Bearer <token>` on every call.

## Steps
1. `set_reference_targets` (POST /v2/reference-targets) - set the location and details of a reference location or object, or use `set_reference_target_current_location` (POST /v2/reference-targets/current-location) to anchor the robot's current position.
2. `reference_targets` (GET /v2/reference-targets) - list all previously set reference targets to confirm the write.
3. `polymath_feedback` (GET /v2/polymath-feedback) - read combined autonomy, navigation, and vehicle feedback to see the robot's current state relative to targets.

## Rules
- Coordinates are GeoPoints (lat/lon); see data-model/polymath-data-model.yml for the entity relationships.
- Validation failures return 422 with a `detail[]` list of field errors.
