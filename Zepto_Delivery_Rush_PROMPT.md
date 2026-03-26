# 🚀 Zepto Delivery Rush — Production Build Prompt

---

## 🎯 OBJECTIVE

Build a **single-file, mobile-first interactive web game** that simulates a Zepto delivery journey — from order pickup to final delivery.

The experience should feel:
- Fast-paced ⚡
- Realistic 🚴‍♂️
- Fun + chaotic 😂
- Rewarding 🎯

---

## 📱 PLATFORM

- Mobile-first (390×844)
- Single `index.html`
- No external dependencies
- Vanilla HTML + CSS + JavaScript
- Must run instantly (offline compatible)

---

## 🎨 BRAND SYSTEM

### Visual Direction
- Premium dark UI
- Inspired by Zepto brand

### Colors
- Deep Purple (primary background)
- Coral → Orange gradient (accent)
- White text
- Glassmorphism surfaces

---

## 🎮 GAME STRUCTURE

### Scene Flow (10 Scenes)

1. Boot Splash  
2. Order Card  
3. Grocery Picking  
4. Bike Delivery (core gameplay)  
5. Arrival  
6. Dial Screen  
7. Customer Call  
8. Elevator  
9. Corridor  
10. Result Screen  

---

## 🧩 SCENE BREAKDOWN

---

### Scene 1 — Boot Splash
- Animated entry
- Brand intro
- CTA to start

---

### Scene 2 — Order Card
- Display:
  - Customer name
  - Order items
  - Delivery location
- Accept interaction

---

### Scene 3 — Grocery Picking

**Interaction:**
- Tap correct items
- Avoid decoys

**UI:**
- 3 shelf layout
- Bottom basket = **brown Zepto paper bag**
- Show Zepto logo

**Feedback:**
- Correct → fly to bag
- Wrong → shake + reject

---

### Scene 4 — Bike Delivery (CORE GAME)

#### Player System
- Rider on motorbike (NOT phone)
- Delivery bag on back (Zepto branding)

#### Controls
- Tap & HOLD left/right
- Smooth drifting
- Lean animation (tilt up to ~20°)

#### Environment
- Road with perspective
- Buildings in background (blend with theme)
- Speed gradually increases

#### Obstacles
- Cars (same direction)
- Few oncoming vehicles
- Bikes
- Dogs 🐕
- Pedestrians 🚶
- Potholes

#### Traffic Logic
- ~80–85% same direction
- ~15–20% oncoming

#### Audio
- Engine sound (loop)
- Dog bark
- Pedestrian shout (“Oye!”)

---

### 🚦 Signal System

**Flow:**
1. Show junction visually
2. Show red signal

**Choice:**
- Jump signal
- Wait

**If Jump:**
- Crash animation
- Message:
  “Always follow the green signal 🟢”

---

### Scene 5 — Arrival

- Show correct phone number
- No scrambling here

**Interaction:**
- “View Number”
- Swipe right → go to dial screen

---

### Scene 6 — Dial Screen

**Mechanic:**
- Keypad numbers are shuffled
- User must dial correct number

**Flow:**
1. Show correct number at top
2. User inputs via scrambled keypad
3. Swipe to call

---

### Scene 7 — Customer Call

#### Options (5 total)
- “Hi, your Zepto order is here”
- “Your Maggi is getting VIP treatment 😎”
- “Bhai jaldi aao”
- “Can you please come down?”
- One neutral/funny option

#### Logic
- Emoji reaction changes based on choice
- “Come down” option → rating penalty

#### UI
- No pre-highlight
- Highlight only on tap

---

### Scene 8 — Elevator

**Interaction:**
- Choose floor

**Wrong Floor:**
- Funny scenarios:
  - Aunty confusion
  - Kid shouting
  - Dog barking
  - Neighbor interaction

**Correct Floor:**
- Smooth transition

---

### Scene 9 — Corridor

**Layout:**
- 4 doors
- Center walkway gap

**Interaction:**
- Tap door

**Wrong Door:**
- Funny character reveal

**Correct Door:**
- Customer appears
- Tap to hand over order

---

### Scene 10 — Result Screen

Display:
- Star rating ⭐
- XP earned
- Performance breakdown:
  - Time
  - Mistakes
  - Signal penalties

**CTA:**
- Play again
- Share option

---

## ⚙️ CORE SYSTEMS

---

### Timer System
- Display: 10:00
- Actual: ~2.5 minutes
- Adjustable via multiplier

---

### Mood System
- Customer response affects:
  - Avatar reaction
  - Final rating
- Persists across scenes

---

### Score System
- Combo logic
- XP calculation
- Star rating (1–5)

---

### Replay System
- Seed-based randomness:
  - Items
  - Customers
  - Floors
  - Numbers

---

## 🔊 AUDIO SYSTEM

Use Web Audio API for:
- Engine loop
- UI taps
- DTMF tones
- Collision sounds
- Reward sounds

---

## 🎉 EFFECTS

- Confetti on high score
- Particle effects (crash, pickups)
- Shake feedback on error

---

## ⚠️ CONSTRAINTS

- No external CDNs
- No React / frameworks
- Smooth performance (60fps)
- No random scene switching
- Scene progresses ONLY after completion

---

## 🧠 EXPERIENCE GOAL

User should feel:
- Pressure ⏱️
- Engagement 🎮
- Fun 😂
- Achievement 🏆

---

## 🔥 OUTPUT

Return a **single fully functional HTML file** with:
- Inline CSS
- Inline JavaScript
- All scenes connected
- Fully playable

---

## 🎯 FINAL OUTCOME

A **campaign-ready Zepto gamified experience** that can:
- Be shared easily
- Run instantly
- Drive engagement

---

## 🏁 TAGLINE

“Delivery in 10 minutes? Try doing it yourself.”
