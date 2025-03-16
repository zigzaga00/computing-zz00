# 🌏 Quakes in the Night - Alarm! 🌏

---

## **Lesson Plan: Creating an Earthquake Alarm with Micro:bit**  
**Duration:** 60 minutes  
**Age Group:** 10 years old  
**Prior Knowledge:**  
- Experience using Micro:bits with MakeCode  
- Understanding of Boolean logic (`and`)  
- Basic event-driven programming  

## **Lesson Objectives:**  
By the end of the lesson, children will:  
1. Review Boolean `and` logic.  
2. Understand how to use the accelerometer and light sensor in Micro:bit.  
3. Follow a modelled coding demonstration to program an earthquake alarm.  
4. Recreate and adapt the project to make it their own.  

---

## **Lesson Structure**

### **1. Starter Activity (5 mins) – Boolean `and` Review**  
- Display two statements on the board:  
  - *It is raining* AND *I have an umbrella* → *I stay dry*.  
  - *It is dark* AND *I turn on a torch* → *I can see*.  
- In pairs, children create their own real-world *AND* examples.  
- Class discussion: Why must both conditions be true for the result?  

---

### **2. Modelled Coding Demonstration (10 mins)**  
- Introduce the challenge: **An earthquake alarm that detects shaking at night.**  
- Live coding in MakeCode, talking through each step:  

#### **Step 1: Create the `isShaking` Variable**  
> "We need to detect when the Micro:bit shakes, but we don’t want it to stay on forever. We’ll create a variable called `isShaking` and use an event to set it to `true`."  
- **Drag in** `on shake` block.  
- **Set** `isShaking = true`.  
- **Pause** 2 seconds (so it doesn't stay true forever).  
- **Set** `isShaking = false`.  

#### **Step 2: Write the Main Algorithm**  
> "Now, we check if it’s both dark AND shaking. If yes, turn on the LEDs. Otherwise, turn them off."  
- **In `forever` loop**, use `if` statement:  
  - Condition: `light level < 100 AND isShaking == true`.  
  - **If true**, show LEDs.  
  - **Else**, clear screen.  

#### **Step 3: Download and Test**  
- Demonstrate downloading to a Micro:bit.  
- **Test shaking in bright light** (nothing happens).  
- **Test shaking in the dark** (alarm triggers).  

> "Now it's your turn! Follow these steps, then make the project your own."

>[!NOTE]
>The video in our shared area can be used for this modelled programming part of the lesson if preferred 😃

---

### **3. Independent Coding (25 mins)**
- **Children recreate the modelled code** in MakeCode.  
- **Once successful, they adapt it:**  
  - **Less Confident:** Work with step-by-step support, using fixed values.  
  - **Average:** Test and debug different thresholds.  
  - **More Confident:** Add sound and a `lightThreshold` variable (adjusted with buttons A/B).  

---

### **4. Showcase and Discussion (15 mins)**  
- **Pairs test each other’s projects.**  
- Discuss real-world applications of earthquake alarms.  
- **Challenge Questions:**  
  - Where could this be useful?  
  - What else could the alarm do to wake people up?
