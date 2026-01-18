## Dementors Game 

**Dementors** is a 2-level platformer game built using **Kaboom.js + TypeScript**, where you control a Kirby-inspired character who can **inhale enemies** and **shoot a powerful star attack**.

The game includes multiple enemy types, scene-based level switching, player health + respawn mechanics, and smooth camera follow — creating a fun survival experience with an eerie theme.

---

## 🧩 Why is the game called “Dementors”?

The name **Dementors** comes from the terrifying creatures in the *Harry Potter* universe.

Dementors are:

- Creatures that cause intense despair and emotional darkness   
- Feared for their ultimate attack: **“The Dementor’s Kiss”**, which removes the soul   
- Described by **J.K. Rowling** as metaphors for **depression**

This game borrows that idea of **survival under pressure** — where enemies feel like unstoppable threats, and the player must fight back and escape through the levels.

---

## 🎮 Demo 

### ✅ Gameplay Screenshot 
![game preview](preview.png)

🔗 **Live Demo:** https://thedementors.netlify.app/

---

## ✨ Features

### 🕹️ Core Gameplay
- ✅ Player movement (Left / Right)
- ✅ Jump + **Double Jump**
- ✅ **Inhale mechanic** to consume enemies
- ✅ **Star shooting attack** after inhaling
- ✅ Camera follows player smoothly

### 👾 Enemy System
Includes multiple enemies with unique behaviors:
- 🔥 **Flame Enemy**: jumps at intervals
- 🧍 **Guy Enemy**: moves left & right (patrolling enemy)
- 🐦 **Bird Enemy**: spawns continuously and flies across the map at random speeds

### 🗺️ Level & Scene System
- ✅ Two playable levels: **Level 1** and **Level 2**
- ✅ Levels are built using a **map-based system**
- ✅ Player progresses by reaching the **exit portal**
- ✅ Scene switching is handled automatically

### ❤️ Health & Respawn
- ✅ Player starts with **3 HP**
- ✅ Colliding with enemies reduces health
- ✅ If HP reaches 0 → scene reloads (player respawns)
- ✅ If player falls off the map → respawns

---

## 🎮 Controls

| Key | Action |
|-----|--------|
| ⬅️ Left Arrow | Move Left |
| ➡️ Right Arrow | Move Right |
| **X** | Jump (Double Jump enabled) |
| **Z** | Inhale enemies / Shoot Star Attack |

### ⭐ Inhale + Star Attack Logic
- Hold **Z** to inhale
- Nearby enemies become inhalable
- Once an enemy is inhaled, the player becomes **full**
- Release **Z** to shoot a **star projectile**
- Star projectile destroys enemies on collision

---

## 🧠 Game Mechanics

### 🎭 Player States
The game uses different player states to manage gameplay actions:

- **idle / run**
- **jump**
- **inhale**
- **full** (after inhaling)
- **shooting star attack**
- **hit / damaged**
- **respawn logic**

---

### 💥 Collisions & Damage System
- Enemy collisions trigger a **damage event**
- Player health decreases by **1**
- If player HP reaches **0** → the game resets the current level

---

### 🪂 Falling Detection
If the player falls below a certain position (off the map), the game reloads the scene and respawns the character.

---

## 🛠️ Tech Stack

- **Kaboom.js** (2D game engine)  
- **TypeScript**  
- **Scene-based design**  
- **Map-based level system**  

---

## How to run the project ?

Assuming you have `node` installed.
- Install dependencies with `npm install`
- Run locally with `npm run dev`
- Build for production with `npm run build` and a dist folder should appear

