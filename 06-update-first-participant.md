# API Test 06 — Update First Participant

## Task

Update the information of the first participant and verify the updated data using the participant ID.

## Participant

**Participant ID:** 182  
**Expedition ID:** 108

## Step 1 — Update Participant

**Method:** PUT

**Endpoint:** `https://api.realbugz.com/participants/182`

### Updated Data

Name: Thomas A Anderson  
Role: leader  
Specialization: Explorer  
Experience: 5  
Expedition ID: 108

### Expected Result

The participant information is successfully updated.

### Actual Result

The participant was successfully updated.

**Participant ID:** 182

---

## Step 2 — Verify Updated Participant

**Method:** GET

**Endpoint:** `https://api.realbugz.com/participants/182`

### Expected Result

The API returns the updated participant information.

### Actual Result

The participant was returned successfully with the following data:

**Name:** Thomas A Anderson  
**Role:** leader  
**Specialization:** Explorer  
**Experience:** 5  
**Participant ID:** 182  
**Expedition ID:** 108

### Result

**PASS**
