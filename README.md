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
| Mouse Drag        | Look around (optional)           |

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

## 🎥 **Camera System**
- Smooth camera follow with collision prevention to avoid passing through objects.  
- Adjustable camera height and distance using parameters.

---

## 🚀 **Project Setup & Configuration**
### 🎯 **Step 1: Download or Clone the Project**
```bash
git clone https://github.com/yourusername/Gravity-Controller.git
```
Or manually download the project from GitHub.

---

### 🛠️ **Step 2: Open Project in Unity**
1. Open Unity Hub.
2. Click **Open Project**.
3. Select the project folder.
4. Open the `SampleScene` or relevant scene.

---

### ⚙️ **Step 3: Assign Required Components**
#### 1. **Player Model Setup**
- Drag your 3D Player Model into the scene.
- Add the following components:
    - `Rigidbody`
    - `Capsule Collider` (or appropriate collider)
    - `PlayerMovement` script.

#### 2. **Animator Setup**
- Create an Animator Controller.
- Add `Idle` and `Run` animations to the controller.
- Add `Animator` to the Player and assign the created controller.

---

### 🎮 **Step 4: UI Setup (Optional)**
- Create a **Canvas** for the UI.
- Add a `TextMeshPro` element for the timer and result message.
- Link the `TimerController` script to this UI.

---

## ⚡ **Customization Options**
### 🎨 **Movement Speed & Jump Power**
- Open `PlayerMovement.cs`.
- Modify these public variables in the Inspector:
```csharp
public float moveSpeed = 5f;         // Speed of movement
public float jumpForce = 7f;         // Jump force strength
```

### 🌌 **Gravity Rotation Speed**
- Modify this value to control how smoothly the character rotates after gravity changes:
```csharp
public float rotationSpeed = 5f;     // Speed of smooth rotation
```

### 🎥 **Camera Settings**
- Open `CameraCollisionHandler.cs` to change camera distance and height:
```csharp
public float distanceFromPlayer = 5f;  // Distance from player
public float cameraHeight = 2f;        // Camera height above player
```

### ⏳ **Idle Delay Before Animation Switch**
- Modify the delay before switching to idle animation:
```csharp
public float idleDelay = 1f;         // Delay before returning to idle
```

---

## 📝 **How to Add Your Animations**
1. Drag your FBX models for **Run** and **Idle** into the Unity project.
2. Create an Animator Controller (if not created yet).
3. Add the animations to the Animator.
4. Set up a `float` parameter called `Speed` and link conditions:
    - **Run:** When `Speed > 0.1`
    - **Idle:** When `Speed <= 0.1`
5. Assign the Animator Controller to your Player.

---

## 🎯 **Win/Fail Setup**
1. Create a cube (or any GameObject) as the **Finish Line**.
2. Add a `Box Collider` with `Is Trigger` enabled.
3. Attach the `Finish.cs` script to the cube.
4. Ensure the `Finish Line` has the tag `Finish`.

---

## 🏆 **Future Improvements**
- Add wall-running and parkour mechanics.
- Implement multiple levels with increasing difficulty.
- Add visual effects when gravity shifts.

---

## 📚 **References**
- Unity Official Docs: [https://docs.unity3d.com/](https://docs.unity3d.com/)  
- TextMeshPro Setup: [https://docs.unity3d.com/Packages/com.unity.textmeshpro](https://docs.unity3d.com/Packages/com.unity.textmeshpro)  

---

## 💬 **Contact**
For questions or contributions, feel free to reach out! 😎

---

## 🎉 **Happy Gaming!**
```bash
Made with ❤️ in Unity by [Your Name/Username]
```

---

## 🧩 **File Structure Overview:**
```
/Assets
├── /Animations
│   ├── Run.fbx
│   └── Idle.fbx
├── /Scripts
│   ├── PlayerMovement.cs
│   ├── TimerController.cs
│   ├── Finish.cs
│   └── CameraCollisionHandler.cs
└── /UI
    └── TimerUI.prefab
```

---

## 📢 **Final Notes**
- Make sure all references are assigned correctly in the Unity Inspector.
- Test different gravity configurations to ensure a smooth experience.

🔥 Now your `README.md` is ready to impress everyone! Let me know if you need any more tweaks or improvements! 😎🚀
