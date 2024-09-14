### **Pixel Party: Creating and Customizing Simple Animations (One-Hour Lesson)**

**Objective**: By the end of this lesson, students will create a simple animation using the LED display on the micro:bit, customize it with their own ideas, and refine the animation for smooth transitions.

The online coding is to be developed using the [makecode editor](https://makecode.microbit.org/#editor)

---

### **Lesson Outline**

#### **1. Introduction (15 minutes)**
- **Explanation**: Introduce the concept of animation by explaining how displaying multiple images in quick succession can create the illusion of movement. Use a real-world example, like a flipbook.
- **Demo**: Show a simple animation on the micro:bit, such as a smiley face that blinks or a ball that moves across the screen. Highlight the code that switches between two or more images.

>[!NOTE]
>At this point in the lesson the video in our shared area could be used as it shows the students how to create animations and progresses the complexity for less to more confident programers

#### **Key Concepts**:
- Displaying multiple images using `basic.showLeds()`
- Adding a delay between images using `basic.pause()`
- Using `basic.forever()` to repeat the animation

#### **Example Code**:
```javascript
basic.forever(function () {
    basic.showLeds(`
        . . . . .
        . # . # .
        . . . . .
        # . . . #
        . # # # .
    `)
    basic.pause(300)
    basic.showLeds(`
        . . . . .
        # . # . #
        . . . . .
        . # # # .
        . . . . .
    `)
    basic.pause(300)
})
```

---

#### **2. Main Activity: Creating a Custom Animation (40 minutes)**
- **Task**: Students will create a looping animation of at least three frames. It could be a simple animation such as a character jumping, a car driving, or a heart beating.
  
##### **Steps**:
1. **Frame Design**: Students draw three different images that will appear on the LED display, each representing a different “frame” of their animation.
2. **Coding**: Students code the three images in sequence, adding `basic.pause()` between each frame to control the timing of the animation.
3. **Looping**: Use `basic.forever()` to repeat the animation indefinitely, creating a continuous loop.

---

#### **3. Differentiation**:

- **Less confident programmers**: 
  - The children use `show icon` pictures instead of creating their own using `show leds`.
  - Focus on completing a two-frame animation, such as a simple flashing icon. Assist with adjusting the pause timing for smoothness.
  
- **Average ability programmers**:
  - Encourage them to design three or more frames and explore how different pause lengths affect the speed of the animation.
  - Allow them to experiment with different image designs to create an interesting story or effect (e.g., a ball bouncing).
  
- **More confident programmers**:
  - Challenge them to create a smooth, seamless animation. They should design at least four frames and refine their animation by adjusting the timing between different frames.
  - Encourage them to make more complex animations, like a character walking or a rocket exploding.
  - Introduce the concept of optimizing frame rates for different parts of the animation (e.g., faster during some parts, slower during others).

---

#### **4. Plenary and Reflection (5 minutes)**
- **Showcase**: Selected children present their animation to the class, explaining what they made and how they adjusted the timing and frames to create their effect.
- **Discussion**: Ask reflective questions such as:
  - "How did the pause timing affect the speed of your animation?"
  - "What changes did you make to improve your animation?"

---

This lesson provides a balance of creativity, coding practice, and progression for all skill levels, while allowing students to engage in a fun, visual project.
