# Test Report — Major Mayhem Clone

**Project:** Major Mayhem Clone (Unity)  
**Build Version:** v1.0 (APK)  
**Report Date:** 2025-09-18  
**Tester:** Arystan Akshulakov  

---

## 1. Test Scope
This round of testing covered:
- Core gameplay mechanics (running, shooting, checkpoints, HP system)  
- UI and navigation (menus, buttons, victory screen)  
- Visuals and audio (animations, sound effects, popups)  
- Stability and performance 
- Pre-submit checks (store readiness, versioning, build packaging)  

---

## 2. Test Execution Summary
- **Test Cases Executed:** 10  
- **Passed:** 7  
- **Failed:** 3  
- **Blocked/Skipped:** 0  

**Execution Status:**  
| Status   | Count |
|----------|-------|
| ✅ Passed | 7     |
| ❌ Failed | 3     |
| ⏸ Skipped| 0     |

---

## 3. Bugs Found
| Bug ID   | Title                                      | Severity | Status   |
|----------|--------------------------------------------|----------|----------|
| [BUG-001](bug-reports/BUG-001.md) | Character loses 2 HP from single hit     | Major    | Open     |
| [BUG-002](bug-reports/BUG-002.md) | Headshot popup does not disappear        | Minor    | Open     |
| [BUG-003](bug-reports/BUG-003.md) | "Play Again" button not clickable (UWP)  | Major    | Open     |

---

## 4. Checklist Results
- Installation & Launch: ✅ Passed  
- UI & Navigation: ❌ Failed (BUG-003)  
- Core Gameplay: ❌ Failed (BUG-001, BUG-002)  
- Visuals & Audio: ✅ Passed (except BUG-002)  
- Performance & Stability: ✅ Passed  
- Pre-Release Checks: ✅ Passed (excluding open bugs)  

---

## 5. Overall Assessment
The game is **stable on Android and iOS**, with core gameplay functioning correctly in most scenarios.  
However:  
- Critical issue with health system (BUG-001) affects balance.  
- UI issue (BUG-003) blocks replay functionality.  
- Minor issue with visuals (BUG-002) impacts polish.  

**Release Readiness:** ❌ Not ready for submission until major bugs are fixed.  

---

## 6. Recommendations
1. Fix BUG-001 and BUG-003 before submission (blockers for gameplay and platform compliance).  
2. Fix BUG-002 to improve user experience, though it’s not release-blocking.  
3. Perform a regression test on HP system and replay functionality after fixes.  
4. Re-run full test before pre-submit checks.  
