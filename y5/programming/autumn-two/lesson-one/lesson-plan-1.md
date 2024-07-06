### Lesson Sequence: Creating a Fish Collecting Game in Scratch Using Clones

**Project Overview:** Students will create a game where a cat sprite moves up and down to collect fish sprites that appear as clones moving across the screen. The game will include a timer controlled by a variable, a score system, and different responses based on the fish costumes.

#### Lesson 1: Introduction to X and Y Coordinates, Basic Movement, and Cloning

**Objective:** Students will learn about X and Y coordinates in Scratch, create basic movement for the cat sprite, and introduce cloning for the fish sprites.

**Materials Needed:** Computers with Scratch installed | projector for demonstration.

---

**Lesson One:**

1. **Introduction (20 minutes):**
   - Explain the game project | show a simple [example project](https://scratch.mit.edu/projects/1043382647/)
   - Introduce X and Y coordinates using a projector to show the Scratch stage.
   - Demonstrate how the X axis (horizontal) and Y axis (vertical) work.
   - Introduce the concept of cloning in Scratch.
   - If not confident with the above - please use the video in the shared area 😃

2. **Activity (35 minutes):**
   - **All Students:**
     - Create a new Scratch project.
     - Add a cat sprite and use arrow keys to move it up and down using the Y coordinate.
       ```scratch
       when [up arrow v] key pressed
       change y by 10

       when [down arrow v] key pressed
       change y by -10
       ```
     - Add a fish sprite and create clones of the fish that move across the screen.
       ```scratch
       when green flag clicked
       forever
         create clone of [myself v]
         wait 1 seconds
       end

       when I start as a clone
       set rotation style left-right
       point in direction -90
       go to x: 240 y: (pick random -180 to 180)
       repeat until <x position < -240>
         move 5 steps
       end
       delete this clone
       ```
   - **Differentiation:**
     - **Less Confident Programmers:**
       - Focus on understanding basic movement and cloning with access to screenshots of how to implement the code.
     - **Average Ability Programmers:**
       - Experiment with different movement steps to control fish clone speed | different y values for the cat | different clone intervals for fish | different costumes for clones of fish.
     - **More Confident Programmers:**
       - Implement boundary checks to prevent the cat sprite from moving off the screen and add more complex movement patterns for the fish clones such as zig-zaging.

3. **Review and Sharing (5 minutes):**
   - Discuss what was learned.
   - Allow a few students to share their progress.

---

>sometimes it is the people no one can imagine anything of who do the things no one can imagine - alan turing
