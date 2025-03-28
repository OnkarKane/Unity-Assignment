# Unity-Assignment
Got it! 🎯 Let's make an awesome, detailed, and clean `README.md` that highlights your project! 😎🚀

---

# 🎮 **Gravity Manipulation 3D Player Controller**  
A 3D Player Controller built in Unity that allows smooth WASD movement, gravity manipulation, and mouse-controlled gravity changes. The player can jump, rotate, and even reverse gravity dynamically!

---

## 📌 **Features**
✅ Smooth WASD movement relative to the player’s direction.  
✅ Gravity changes using `Ctrl + Mouse Drag` with smooth character rotation.  
✅ Correct alignment of the character's feet when gravity shifts.  
✅ Look left and right using `Q` and `E` (or mouse drag).  
✅ Double jump functionality.  
✅ Idle and Run animations for character movement.  
✅ Countdown timer to complete the level before time expires.  
✅ Win and Game Over conditions based on finishing time or reaching the target.  
✅ Smooth camera with collision prevention to avoid clipping through walls.

---

## 🕹️ **Controls**
| Key/Action        | Description                      |
|------------------|----------------------------------|
| `W` / `A` / `S` / `D` | Move forward, left, back, right |
| `Space`           | Jump (Double jump enabled)      |
| `Q`               | Rotate 90° left                 |
| `E`               | Rotate 90° right                |
| `Ctrl + Mouse Drag` | Change gravity (on mouse release) |
| `Ctrl + Drag Up`  | Gravity flips upwards (180° flip) |
| `Ctrl + Drag Down`| Gravity flips down               |
| `Ctrl + Drag Right` | Gravity shifts right             |
| `Ctrl + Drag Left`  | Gravity shifts left               |


---

## 🌌 **How Gravity Manipulation Works**
1. Hold `Ctrl` and drag the mouse in any direction.
2. Release the mouse to change gravity.
3. The character rotates smoothly and lands perfectly aligned to the new gravity direction.
4. Gravity is dynamically applied, keeping the object grounded properly on all surfaces.

---

## 🎥 **Animations**
- **Idle:** When no keys are pressed.  
- **Run:** Triggered automatically when the player moves using `W`, `A`, `S`, or `D`.  
- Animation transitions include a slight delay before switching back to idle to maintain smoothness.

---

## 🕒 **Timer System**
- A countdown timer starts when the level begins.
- Objective: Reach the `Finish Line` before the timer expires.
- **Win Condition:** Touch the `Finish Line` GameObject.
- **Lose Condition:** Timer expires without reaching the target.

---

## Shortcomings 
I couldnt get a non clipping Camera to work and I couldnt get the Halo to work 


