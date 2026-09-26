# API Test 04 — Create and Verify New Expedition

## Task

Create a new expedition and verify its existence using the generated ID.

## Step 1 — Create Expedition

**Method:** POST

**Endpoint:** `https://api.realbugz.com/expeditions/`

### Request Body

Name: New test Expedition  
Start date: 2026-09-25  
End date: 2026-09-30  
Status: planned  
Description: API test expedition  
Location: Nha Trang  
Budget: 1500.0

### Expected Result

A new expedition is created and receives its own ID.

### Actual Result

**Status Code:** 200

The expedition was successfully created.

**Expedition ID:** 108

---

## Step 2 — Verify Expedition

**Method:** GET

**Endpoint:** `https://api.realbugz.com/expeditions/108`

### Expected Result

The newly created expedition exists and its details are returned.

### Actual Result

**Status Code:** 200

The API returned the newly created expedition.

**Expedition ID:** 108  
**Name:** New test Expedition  
**Budget:** 1500.0  
**Location:** Nha Trang  
**Status:** planned

### Result

**PASS**
