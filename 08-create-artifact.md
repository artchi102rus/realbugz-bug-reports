# API Test 08 — Create Artifact

## Task

Create an artifact discovered during the expedition and verify its existence using the artifact ID.

## Artifact

**Name:** Ancient Compass
**Artifact ID:** 88
**Expedition ID:** 108
**Discovery Date:** 2026-09-26
**Condition:** excellent
**Estimated Age:** 500 years
**Location:** Nha Trang

---

## Step 1 — Create Artifact

**Method:** POST

**Endpoint:** `https://api.realbugz.com/artifacts/`

### Request Body

**Name:** Ancient Compass
**Description:** An ancient compass discovered during the expedition
**Discovery Date:** 2026-09-26
**Condition:** excellent
**Estimated Age:** 500
**Location:** Nha Trang
**Expedition ID:** 108

### Expected Result

The artifact is successfully created and receives its own unique ID.

### Actual Result

The API returned **200 OK**.

The artifact was successfully created.

**Artifact ID:** 88

---

## Step 2 — Verify Artifact Exists

**Method:** GET

**Endpoint:** `https://api.realbugz.com/artifacts/88`

### Expected Result

The API returns the artifact data using its ID.

### Actual Result

The API returned **200 OK**.

The returned artifact has the following data:

**Name:** Ancient Compass
**Artifact ID:** 88
**Expedition ID:** 108
**Discovery Date:** 2026-09-26
**Condition:** excellent
**Estimated Age:** 500
**Location:** Nha Trang

The artifact exists and is correctly associated with expedition 108.

### Result

**PASS**
