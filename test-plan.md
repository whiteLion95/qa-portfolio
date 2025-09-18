# Test Plan – Major Mayhem Clone

## 1. Introduction
The purpose of this document is to define the testing approach, scope, and deliverables for the mobile game **Major Mayhem Clone**, developed in Unity.  
The objective is to verify that the core gameplay mechanics, user interface, animations, and overall user experience meet the expected quality standards before release.

---

## 2. Scope of Testing

### In Scope
- Core gameplay mechanics:
  - Auto-run movement.
  - Checkpoint hiding system.
  - Shooting and headshot logic.
  - Enemy spawn, movement, and attack behavior.
  - Player HP system and game-over condition.
  - Victory animation and "Play Again" button.
- UI elements and text:
  - "Headshot" popup.
  - HP indicators.
  - Buttons and menus.
- Audio (if implemented).
- Compatibility with target platforms (Android).

### Out of Scope
- Multiplayer functionality (not implemented).
- Monetization systems (not implemented).
- Advanced performance/stress testing.

---

## 3. Test Objectives
- Ensure functional correctness of all implemented game mechanics.  
- Validate UI/UX behavior for clarity and responsiveness.  
- Verify stability on supported platforms.  
- Detect and document bugs with reproducible steps.  

---

## 4. Test Strategy
### Types of Testing
- **Functional Testing** – validation of mechanics, UI, and rules.  
- **Exploratory Testing** – ad-hoc play sessions to uncover unexpected issues.  
- **Regression Testing** – re-execution of core test cases after fixes.  
- **Smoke Testing** – quick verification of build stability.  
- **Compatibility Testing** – running the game on multiple devices/OS versions.  

### Test Levels
- **Unit testing**: not in QA scope (covered by developers if needed).  
- **Integration testing**: functional testing of combined mechanics (e.g., headshot → death animation → popup).  
- **System testing**: end-to-end validation on real devices.  

---

## 5. Test Deliverables
- Test Cases (Excel format).  
- Checklists (Markdown format).  
- Bug Reports (Markdown format with screenshots/videos).  
- Test Report (summary of executed tests, pass/fail ratio, open defects).  
- Exploratory Testing Notes.  

---

## 6. Test Environment
- **Devices:**  
  - Android: Samsung Galaxy A52 (Android 12), Pixel 4a (Android 13)
- **Builds:** APK files delivered by developer (internal build).  
- **Tools:**  
  - Test case management: Google Sheets / Excel.  
  - Bug tracking: simulated Jira-style bug reports.  
  - Screen recording: OBS / built-in device recorder.  

---

## 7. Entry & Exit Criteria

### Entry Criteria
- Playable APK build delivered.  
- Basic documentation available (controls, features).  
- Environment set up on test devices.  

### Exit Criteria
- All high/critical severity bugs are fixed or deferred with justification.  
- ≥95% of planned test cases executed.  
- Core gameplay features verified as stable.  
- Test report delivered.  

---

## 8. Risks & Mitigations
- **Risk:** Limited device coverage.  
  - *Mitigation:* Use Android emulator in addition to physical devices.  
- **Risk:** Short testing timeline.  
  - *Mitigation:* Prioritize smoke and core gameplay test cases.  
- **Risk:** Lack of design documentation.  
  - *Mitigation:* Perform exploratory testing and align with developer expectations.  

---

## 9. Schedule
- **Test planning:** Day 1.  
- **Test case creation:** Day 2.  
- **Test execution:** Days 3–5.  
- **Bug reporting & retesting:** Days 3–6.  
- **Test report delivery:** Day 7.  

---

## 10. Approval
- QA Engineer: Arystan Akshulakov  
- Developer: Arystan Akshulakov
- Stakeholder: *N/A (demo project for portfolio)*  
