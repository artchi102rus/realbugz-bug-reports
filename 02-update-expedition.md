# API Test 02 — Update Expedition

## Task

Update the expedition created in the previous step and verify that the details were successfully updated.

## Step 1 — Update Expedition

**Method:** PUT

**Endpoint:** `https://api.realbugz.com/expeditions/108`

### Request Body

Name: Test Expedition update  
Start date: 2026-09-25  
End date: 2026-09-30  
Status: planned  
Description: API test expedition  
Location: Nha Trang  
Budget: 2000.0

### Expected Result

The expedition details are successfully updated.

### Actual Result

**Status Code:** 200

The expedition was successfully updated.

**Expedition ID:** 108

---

## Step 2 — Verify Updated Expedition

**Method:** GET

**Endpoint:** `https://api.realbugz.com/expeditions/108`

### Expected Result

The API returns the updated expedition details.

The following values should be updated:

**Name:** Test Expedition update  
**Budget:** 2000.0

### Actual Result

**Status Code:** 200

The API returned the updated expedition with ID 108.

**Name:** Test Expedition update  
**Budget:** 2000.0  
**Location:** Nha Trang  
**Status:** planned

### Result

**PASS**
