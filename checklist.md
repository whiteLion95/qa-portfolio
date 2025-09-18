# QA Checklist — Major Mayhem Clone

This checklist covers high-level areas to verify during testing.  
Each item can be marked as [ ] (not tested) or [x] (tested/passed).  

---

## 1. Installation & Launch
- [ ] Game installs successfully on Android devices  
- [ ] Game launches without crashes  
- [ ] Game icon and name displayed correctly on device  
- [ ] Game reaches main menu within 5 seconds  

---

## 2. UI & Navigation
- [ ] All buttons are clickable and responsive  
- [ ] “Start Game” launches the first level  
- [ ] “Play Again” restarts the level after victory  
- [ ] UI elements scale properly on different screen resolutions  
- [ ] Pause menu opens and closes correctly  

---

## 3. Core Gameplay
- [ ] Character auto-runs between checkpoints  
- [ ] Character hides behind crates at checkpoints  
- [ ] Player can shoot by tapping on screen  
- [ ] Enemies spawn correctly at checkpoints  
- [ ] Enemy HP decreases on hit  
- [ ] Headshots kill enemies instantly  
- [ ] Headshot popup appears and disappears after delay  
- [ ] Character loses exactly 1 HP per bullet hit  
- [ ] Game ends when character HP reaches 0  
- [ ] Victory animation plays after last checkpoint  

---

## 4. Visuals & Audio
- [ ] Animations play smoothly (run, shoot, death, victory)  
- [ ] Death animation plays before enemy disappears  
- [ ] Sounds play for shooting, taking damage, and victory  
- [ ] Background music loops without interruptions  
- [ ] Popups (e.g., “HEADSHOT”) appear in correct position  

---

## 5. Performance & Stability
- [ ] No crashes during 30 minutes of continuous play  
- [ ] Game runs at stable FPS (>30) on mid-range devices  
- [ ] No major memory leaks or overheating on mobile  
- [ ] Loading times are under 5 seconds  

---

## 6. Pre-Release Checklist (Pre-Submit)
- [ ] No critical/blocker bugs open  
- [ ] All store metadata (icon, screenshots, description) correct  
- [ ] Game passes platform-specific submission requirements  
- [ ] Version number incremented correctly  
- [ ] Build signed and packaged successfully  
