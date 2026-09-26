# API Test 03 — Delete Expedition

## Task

Delete the expedition created in the first step and verify that it no longer exists.

## Step 1 — Delete Expedition

**Method:** DELETE

**Endpoint:** `https://api.realbugz.com/expeditions/108`

### Expected Result

The expedition is successfully deleted.

### Actual Result

**Status Code:** 200

The expedition was successfully deleted.

**Expedition ID:** 108

---

## Step 2 — Verify Expedition Does Not Exist

**Method:** GET

**Endpoint:** `https://api.realbugz.com/expeditions/108`

### Expected Result

The expedition no longer exists.

The API should return an error indicating that the expedition was not found.

### Actual Result

**Status Code:** 404

The API returned a not found error, confirming that the expedition no longer exists.

**Expedition ID:** 108

### Result

**PASS**
