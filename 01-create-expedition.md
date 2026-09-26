# API Test 01 — Create and Verify Expedition

## Task

Create a new expedition and verify its existence using the generated ID.

## Step 1 — Create Expedition

**Method:** POST

**Endpoint:** `https://api.realbugz.com/expeditions/`

### Request Body

Name: Test Expedition  
Start date: 2026-09-25  
End date: 2026-09-30  
Status: planned  
Description: API test expedition  
Location: Nha Trang  
Budget: 1000

### Expected Result

A new expedition is created and receives a unique ID.

### Actual Result

**Status Code:** 200

The expedition was created successfully.

**Expedition ID:** 108

---

## Step 2 — Verify Expedition

**Method:** GET

**Endpoint:** `https://api.realbugz.com/expeditions/108`

### Expected Result

The created expedition exists and its data is returned.

### Actual Result

**Status Code:** 200

The API returned the expedition with ID 108.

### Result

**PASS**
