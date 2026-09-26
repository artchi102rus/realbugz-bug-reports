# API Test 05 — Create Three Participants

## Task

Create three different participants for the expedition created in the previous step and verify their existence using the expedition ID.

## Expedition

**Expedition ID:** 108

## Created Participants

### Participant 1

**Name:** John Smith  
**Role:** leader  
**Specialization:** Explorer  
**Experience:** 5  
**Participant ID:** 182

### Participant 2

**Name:** Michael Green  
**Role:** geologist  
**Specialization:** Geology  
**Experience:** 7  
**Participant ID:** 183

### Participant 3

**Name:** Anna Brown  
**Role:** historian  
**Specialization:** Biology  
**Experience:** 3  
**Participant ID:** 184

## Verification

**Method:** GET

**Endpoint:** `https://api.realbugz.com/expeditions/108`

### Expected Result

The expedition exists and contains the three created participants.

### Actual Result

**Status Code:** 200

The API returned expedition 108 with three participants:

- John Smith — ID 182
- Michael Green — ID 183
- Anna Brown — ID 184

All three participants are associated with expedition 108.

### Result

**PASS**
