## Screen Time Focus App — “Solar Focus” (Working Title)

**Concept:**  
 A **screen-time management app** that helps users focus and manage device usage through **Live Activities**, **App Intents**, and **Dynamic Island** integration — all wrapped in a **solar system–inspired, space-themed UI**.

---

### **Core Features**

1. ** Solar System Visualization**

   * A **RealityKit 3D solar system model** represents the user’s focus sessions.

   * Each **planet’s orbit speed** corresponds to the **session progress** (e.g., the faster the orbit, the shorter the session).

   * The **Sun** symbolizes focus — planets orbiting smoothly means focus is maintained.

2. **Focus Timer (Live Activity \+ Dynamic Island)**

   * Focus sessions start via **App Intents** (e.g., `StartTimerIntent`).

   * A **Live Activity** shows the ongoing session in the **Dynamic Island**, with:

     * Remaining time

     * Elapsed progress ring

     * Buttons for **Pause** and **Stop**

   * Tapping notifications or island expands the activity UI.

3. **Screen Time Integration**

   * Uses **FamilyControls**, **ManagedSettings**, and **DeviceActivity** frameworks.

   * When a focus session starts:

     * Selected apps get **shielded** (blocked or limited).

     * When ended or paused, the shield is lifted.

   * Includes **custom ShieldActionExtension** to handle resume/pause actions directly.

4. **Smart Notifications**

   * Sends local notifications when:

     * Focus session ends.

     * A user tries to open a blocked app.

     * Time milestones (e.g., halfway or 5 minutes left).

5. **App Intents Integration**

   * Custom intents like:

     * `StartTimerIntent`

     * `PauseTimerIntent`

     * `EndTimerIntent`

   * Enables quick Siri Shortcuts, widgets, or automation triggers.

6. **Visual & Thematic Style**

   * Space-inspired design:

     * Dark starfield backgrounds

     * Animated planetary motion

     * Glowing orbits and ambient lighting effects

   * Consistent with the “focus in space” metaphor — the user’s attention is a celestial system staying in balance.

---

### **Technical Stack**

* **SwiftUI** — Main UI framework.

* **RealityKit** — 3D solar system visualization and animations.

* **AppIntents \+ ActivityKit** — For Live Activity and Dynamic Island interactions.

* **FamilyControls \+ ManagedSettings \+ DeviceActivity** — Screen time and app restrictions.

* **UserNotifications** — For reminders and activity updates.

---

### **Vision**

We want to **raise awareness about screen time** and help people become more conscious of how much time they spend on their devices.  
 Through an engaging **solar system metaphor**, users can *see* their phone usage take shape — as planets orbit, slow down, or drift away, they visualize how attention and time move throughout the day.

The experience encourages **mindful device use**, not by restriction alone, but through **visual reflection and awareness**.  
 By turning screen-time management into a cosmic journey, the app inspires users to find balance between **digital activity and real-world focus** — making self-awareness feel calm, playful, and meaningful.
