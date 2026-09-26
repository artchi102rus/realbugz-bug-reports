# API Test 09 — Check Full Expedition Details

## Task

Retrieve the complete information about the expedition and verify that it contains 2 participants and 1 artifact created during the previous steps.

## Expedition

**Expedition ID:** 108
**Name:** New test Expedition

---

## Step 1 — Get Full Expedition Information

**Method:** GET

**Endpoint:** `https://api.realbugz.com/expeditions/108`

### Expected Result

The API successfully returns the complete expedition information.

The response should contain:

* Expedition ID `108`
* 2 participants
* 1 artifact

### Actual Result

The API returned **200 OK**.

The expedition information was successfully retrieved.

**Expedition ID:** 108

### Participants

**Participant 1:** Thomas A Anderson
**Participant ID:** 182
**Role:** leader
**Specialization:** Explorer
**Experience:** 5

**Participant 2:** Michael Green
**Participant ID:** 183
**Role:** geologist
**Specialization:** Geology
**Experience:** 7

**Total participants:** 2

### Artifact

**Name:** Ancient Compass
**Artifact ID:** 88
**Condition:** excellent
**Estimated Age:** 500
**Location:** Nha Trang

**Total artifacts:** 1

### Result

**PASS**

The complete expedition information was successfully retrieved.

The expedition contains exactly **2 participants** and **1 artifact**, as expected.
