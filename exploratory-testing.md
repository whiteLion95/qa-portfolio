# Exploratory Testing Report — Major Mayhem Clone

**Project:** Major Mayhem Clone (Unity)  
**Build Version:** v1.0 (APK test build)  
**Session Date:** 2025-09-18  
**Tester:** Arystan Akshulakov  
**Duration:** 1 hour exploratory session  

---

## 1. Charter
Explore gameplay flow, UI responsiveness, and edge cases outside of scripted test cases, focusing on:
- HP and damage mechanics  
- Checkpoint transitions  
- Victory/defeat scenarios  
- UI responsiveness during play  

---

## 2. Notes & Observations

### Gameplay & Mechanics
- At one checkpoint, I tapped rapidly on the same enemy. Enemy HP bar sometimes updated with a delay (~0.2s).  
- If the character is shot **at the exact frame** he peeks out of cover, sometimes no damage is applied (suspected invulnerability frame).  
- When at 1 HP: if two bullets hit almost simultaneously, the character instantly dies without HP bar updating (likely related to BUG-001).  

### UI & Navigation  
- Pause menu: once, the **resume button required two taps** to continue. Couldn’t reproduce consistently.  

### Visuals & Audio
- Headshot popup issue confirmed (BUG-002): popup did not disappear after ~1s delay.  
- In some cases, when making two headshots quickly, **two “HEADSHOT” popups overlapped** before fading out.  

### Performance & Stability
- Game ran at ~60 FPS on Pixel 5 test device.  
- Stable performance: no crashes during 30 minutes of continuous play.  
- Load times under 5 seconds.  

---

## 3. Issues Found
- **BUG-001:** Character loses 2 HP from single hit (already logged).  
- **BUG-002:** Headshot popup does not disappear (already logged).  
- **New Observation:** Resume button sometimes requires two taps (not logged, needs repro steps).  
- **New Observation:** Overlapping “HEADSHOT” popups when killing two enemies quickly (needs bug report).  

---

## 4. Coverage vs Test Cases
- Most **core gameplay test cases** were reinforced during exploratory testing.  
- Additional **edge cases not covered by scripted test cases**:  
  - Simultaneous hits at low HP  
  - Popup stacking  
  - Pause menu responsiveness  

---

## 5. Conclusion
Exploratory testing confirmed scripted issues but also revealed **two new potential bugs**:  
- Pause menu “resume” button requiring two taps (intermittent).  
- Overlapping headshot popups when performing rapid headshots.  

**Next Steps:**  
- Attempt to reproduce pause menu issue more consistently.  
- Create bug report for overlapping popups (BUG-004).  
- Retest HP mechanics after fixing BUG-001.  
