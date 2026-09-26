# API Test 07 — Delete Third Participant

## Task

Delete the third participant and verify that the participant no longer exists using the participant ID.

## Participant

**Name:** Anna Brown  
**Participant ID:** 184  
**Expedition ID:** 108

## Step 1 — Delete Participant

**Method:** DELETE

**Endpoint:** `https://api.realbugz.com/participants/184`

### Expected Result

The third participant is successfully deleted.

### Actual Result

The API returned:

**Message:** Participant deleted successfully

The participant was successfully deleted.

**Participant ID:** 184

---

## Step 2 — Verify Participant Does Not Exist

**Method:** GET

**Endpoint:** `https://api.realbugz.com/participants/184`

### Expected Result

The participant no longer exists.

The API should return an error indicating that the participant was not found.

### Actual Result

The API returned:

**Detail:** Participant not found

The participant no longer exists.

**Participant ID:** 184

### Result

**PASS**
