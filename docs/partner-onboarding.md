# Partner Onboarding

This document describes the practical first-step model for integrating with Namazu API.

## Goal

The goal of onboarding is to make integration simple, controlled, and credible.

The first partners are likely to be:
- ministries
- universities
- research groups
- pilot project operators
- mobile app teams
- IoT vendors
- selected enterprise partners

## Phase 1 onboarding model

The initial onboarding model should be manual and partner-oriented.

Each partner receives:

- a `partner_id`
- a staging API key
- a production API key when approved
- example payloads
- one technical contact path

This is better than trying to open a fully self-service developer portal too early.

## Recommended onboarding steps

### 1. Define the partner type

Examples:
- ministry / public sector
- research institution
- mobile app team
- IoT device vendor
- building operator
- enterprise integration partner

### 2. Define the first use case

Examples:
- media feed only
- sensor upload pilot
- building-linked workflow
- dashboard retrieval
- future analysis collaboration

### 3. Issue a staging key

The partner should first test against:
- sample requests
- validation rules
- expected payload structure
- response handling

### 4. Review operational requirements

Confirm:
- request volume expectations
- data format
- error handling
- location / building metadata policy
- any privacy or governance requirements

### 5. Move to controlled production use

Only after successful testing:
- issue production key
- define support contact
- define permitted endpoints
- define operational logging and monitoring

## Suggested v1 partner types

### Media-only partner
Uses:
- `GET /v1/feed`

### Sensor partner
Uses:
- `POST /v1/sensor/upload`

### Dashboard-linked partner
Uses:
- `GET /v1/buildings/{building_id}/results`

## What to avoid early

Do not overcomplicate onboarding with:
- too many auth models
- too many endpoint variants
- too much self-service UI
- unclear data governance rules

At the beginning, simplicity is a strength.

## Strategic note

The onboarding story should reinforce that Namazu is:

- structured
- credible
- controllable
- extensible
- suitable for institutional use

That positioning matters as much as the endpoint design.
