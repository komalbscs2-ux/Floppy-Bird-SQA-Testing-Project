# Floppy-Bird-SQA-Testing-Project
SQA Testing &amp; Bug Tracking Project for Floppy Bird Web Application using Trello

This repository contains the complete Software Quality Assurance (SQA) testing deliverables, bug tracking documentation, SRS analysis, and execution reports for the Floppy Bird Web Application.

---

##  Live Application & Board Links
 **Live Game URL:** [https://nebezb.com/floppybird/]
 **Trello Testing Board:** [https://trello.com/b/oUiAR8Ft/stqa-project-floppy-bird-testing]

---

## 🛠️ SQA Project Overview
 **Role:** Software Quality Assurance (SQA) Tester
 **Testing Period:** July 2026
 **Environment Tested:** Google Chrome / Windows 11
 **Platform Managed:** Trello (For Test Case Management & Defect Logging)

---

## 📁 Uploaded Project Deliverables
The following documentation files have been uploaded directly to this repository:

1. **`SRS_Floppy_Bird.docx`** — Software Requirements Specification & Scope Analysis.
2. **`BugReport_FloppyBird_Fixed.docx`** — Comprehensive Defect Log Matrix (including Bug-01 Critical Ceiling Collision & Bug-02 UI Distortion).
3. **`trello ss document.docx`** — Visual Verification Proofs & Execution Comments for all 10 Test Cases (TC-01 to TC-10).

---

## 📊 Testing Execution Summary

### 1. Test Cases Executed (Trello Board Verification)
A total of 10 test cases were structured, executed, and verified covering core physics, mechanics, input handling, and user interface responsiveness.

 **TC-01: Verify Bird Jump on Click/Tap** — `PASSED ✅`
  * *Observation:* Input triggers instant upward impulse vector without latency.
 **TC-02: Verify Gravity Effect on Idle State** — `PASSED ✅`
  * *Observation:* Constant gravitational acceleration continuously pulls asset down when idle.
  * **TC-03: Verify Pipe Collision Handling** — `PASSED ✅`
  * *Observation:* Game loop terminates instantly upon hit-box overlap with pipe obstacles.
 **TC-04: Verify Score Increment Mechanics** — `PASSED ✅`
  * *Observation:* Score counter increments accurately by +1 upon passing pipe boundaries.
 **TC-05: Verify Ground Collision Handling** — `PASSED ✅`
  * *Observation:* Instant crash state triggered upon lower floor collision.
 **TC-08: Verify High Score Local Storage Persistence** — `PASSED ✅`
  * *Observation:* Top score persists reliably across browser refreshes using client storage.
 **TC-09: Verify High-Frequency Stress Input Handling** — `PASSED ✅`
  * *Observation:* Rapid click flooding processed cleanly without frame drops or game freeze.

---

### 🐛 2. Defect Log & Bug Summary
During rigorous boundary and compatibility testing, two high-priority functional defects were identified and documented:

#### **BUG-01: Missing Top Ceiling Boundary Collision**
 **Severity:** Critical | **Status:** FAILED ❌
 **Summary:** Input flooding allows the bird asset to exit the upper visible screen canvas and fly infinitely into space, bypassing collision mechanics entirely.

#### **BUG-02: UI Layout Distortion on Window Resizing**
 **Severity:** Major / UI | **Status:** FAILED ❌
 **Summary:** Shrinking the browser window to mobile viewports distorts the canvas aspect ratio, causing scoreboard overlap and pipe cropping.
