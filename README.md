# The Cover Band Scene

## Problem
There is a rich community of cover music performers, venues, and music lovers in the Mid-Atlantic region, but there's no central home to quickly and easily find "who's playing in Atlantic City this weekend", "who's playing at Parx Casino tonight?", or "what time do The Benderz play tomorrow?".

## MVP
### Overview
Summit Avenue currently manages multiple performer websites via unique CMS accounts, causing venue data duplication. The goal of the MVP is to create the system that replaces the unique CMS accounts with one centralized system. This system will be the foundation of The Cover Band Scene system.

### Requirements
#### Functional Requirements
##### Auth Features
FR-01: The system shall provide secure authentication for the admin
FR-02: The system shall provide secure authentication for clients
FR-03: The system shall restrict client read access to specific resources determined by the admin

##### Admin Features
FR-04: The system shall allow the admin to delegate resource access.
FR-05: The system shall allow the admin to create, read, update, and delete any band, venue, or event.
FR-06: The system shall allow the admin to bulk add events via JSON or CSV.
FR-07: The system shall validate required fields and show errors if missing or invalid.
FR-08: The system shall check for and prevent duplicate bands, venues, or events.

##### Authorized Client Features
FR-09: The system shall support pagination for events.

#### Non-functional Requirements
NFR-01: The API shall respond to read requests with a p95 latency of ≤ 200 ms.
NFR-02: The API shall maintain ≥ 99.5% uptime for read endpoints.
NFR-03: All communication shall occur over HTTPS.
NFR-04: Public read endpoints shall support caching and pagination.
NFR-05: Admin and client access shall be authenticated and authorized.
NFR-06: The system shall expose metrics for latency, error rate, and availability.
