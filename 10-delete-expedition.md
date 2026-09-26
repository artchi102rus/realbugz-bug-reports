# API Test 10 — Delete Expedition

## Task

Delete the expedition and verify that the expedition no longer exists using its ID.

## Expedition

**Expedition ID:** 108
**Name:** New test Expedition

---

## Step 1 — Delete Expedition

**Method:** DELETE

**Endpoint:** `https://api.realbugz.com/expeditions/108`

### Expected Result

The expedition is successfully deleted.

### Actual Result

The API returned:

**Message:** Expedition deleted successfully

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

The API returned:

**Detail:** Expedition not found

The expedition no longer exists.

**Expedition ID:** 108

### Result

**PASS**
