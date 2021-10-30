# Role-Based Access Control (RBAC)

Date: 2021-10-29

## Status

Accepted

## Context

Users are going to submit information via the portal that can be considered sensitive. Dietary needs and health conditions that users don't want the community to see but want professionals from clinics to view need to be protected.

## Decision

We will use the NCR Security Service to create users and roles for this system. The role will decide the permission level allowed in the firestore database via the portal service.

## Consequences

Developers will need to become familiar with the NCR Security Service for managing users and roles.