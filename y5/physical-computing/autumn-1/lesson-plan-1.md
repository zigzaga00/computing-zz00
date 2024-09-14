## Animate and Interact

### **Lesson Plan**

**Objective:**  
Students will create an animation on the micro:bit that can be controlled using inputs such as buttons and shaking the device. They will build on their previous experience with animations to integrate interactive elements.

>[!IMPORTANT]
>This project highlights the importance of interactivity in programming physical systems and how these skills can be applied to create more complex projects | we need to make our students aware of this

**Materials:**
- Micro:bits (one per student or pair)
- Computers or tablets with micro:bit programming environment (e.g., MakeCode)
- Projector or screen for demonstrations
- Use the [online editor](https://makecode.microbit.org/#editor)
---

#### **Introduction (10 minutes)**

1. **Review Previous Learning:**
   - Briefly review how to use the led display to create animations using ideas from the [review activities](https://github.com/zigzaga00/computing-zz00/blob/main/y5/physical-computing/autumn-1/review-activities.md).
   - Introduce the new project, **Animate and Interact**, explaining that they will now add interactivity to their animations using buttons and shake inputs.
   - Highlight how programming interactivity into physical systems is essential for creating smart devices and innovations like those seen in the Internet of Things (IoT). Emphasize that interactivity allows devices to respond to user inputs and environmental changes, making technology more useful and engaging.

---

#### **Demonstration (10 minutes)**

During the demonstration we show how we can use a simple *input* such as `button a` to start an *animation*. We also need to show our students how we can progress this so different animations can execute when different *input* such as `button b` and `on shake` can be the *events* to run different animations.

>[!NOTE]
>Encourage the students to be creative and try to link their animations - an example would be `button a` shows a car move left to right whilst `button b` shows the car move right to left | another example would be `button a` for a rocket taking off `button b` for it landing and `on shake` to see it explode

If not feeling confident with the demonstration, please use the video in our shared area 😃

---

#### **Main Activity (35 minutes)**

**Differentiated Tasks:**

   - **Less Confident Programmers:**
     - **Task:** Create a simple animation that plays when the A button is pressed.
     - **Instructions:** Use pre-made animations or simple shapes. Focus on using the `show leds` block to create a few frames and use the `on button A pressed` event to start the animation.
     - **Support:** Provide a step-by-step guide and offer examples of simple animations.

   - **Average Programmers:**
     - **Task:** Create an animation that plays when the A button is pressed and another animation that plays when the B button is pressed.
     - **Instructions:** Use the `on button A pressed` and `on button B pressed` events. Design two different animations or sequences. Ensure they understand how to switch between animations.
     - **Support:** Provide sample code snippets and encourage them to experiment with different animations.

   - **More Confident Programmers:**
     - **Task:** Create an interactive animation that plays when the A button is pressed, the B button is pressed, or when the micro:bit is shaken.
     - **Instructions:** Use `on button A pressed`, `on button B pressed`, and `on shake` events. Design multiple animations or interactive elements that respond to different inputs. Encourage creativity with the animations.
     - **Support:** Provide advanced code blocks and offer guidance on how to combine multiple input events effectively.

**Build and Test**
   - Students work on their tasks. Circulate and provide support based on the needs of each group.
   - Encourage students to test their animations frequently and adjust their code based on their observations.

---

#### **Conclusion (5 minutes)**

1. **Showcase and Discuss:**
   - Invite a few students to demonstrate their animations and explain how they incorporated the different inputs.
   - Discuss what worked well and any challenges they faced.

2. **Recap:**
   - Review the key concepts: how to program animations, use button inputs, and detect shakes.

---

This lesson plan builds on previous knowledge while introducing new interactive elements, ensuring that students of all levels can engage with the content and develop their skills further.
