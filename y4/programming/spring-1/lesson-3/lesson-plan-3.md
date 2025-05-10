# **Lesson 3: The Final Confrontation – Coding the End Scene**

**Duration:** 60 minutes
**Lesson Focus:**

* Creating the endgame encounter using **broadcasts**, **sprite visibility**, and **scene switching**
* Using **ask and answer blocks** for a final challenge
* Handling win/lose outcomes based on user input
* Optional: Adding animation or visual flair for confident coders

---

## **Learning Objectives:**

✅ Use broadcasts to control scene changes and sprite visibility
✅ Use `ask` blocks to capture final user input
✅ Evaluate input using `if / else` statements
✅ Create win or lose endings depending on the user’s answer

---

## **Lesson Breakdown**

### ⏱️ **0–10 min: Recap & Hook – “The Final Battle”**

🎮 *Recap the story so far:* The hero has solved the riddles, learned the spell, and now must face Drako!
🎥 *Show a working example* of the final scene:

* The PC sprite touches the vampire castle
* The castle broadcasts `showDrako`, hides
* Background switches
* Drako appears, says a line, asks for the spell
* If input = spell → victory message
* If wrong → game over

✅ *Explain:* Today we’re **finishing the game** and coding a dramatic ending!

The code can be taught in class or the video in our shared area can be used... :smiley:

---

### ⏱️ **10–25 min: Coding the Trigger and Scene Switch**

**Step 1: Trigger the final scene**

* In the vampire castle sprite:

```scratch
when green flag clicked
show

forever
  if <touching [PC v]> then
    broadcast [showDrako v]
    hide
  end
```

**Step 2: Respond to broadcast in Drako and PC**

* In the **PC sprite**:

```scratch
when I receive [showDrako v]
go to x: 0 y: -100
```

* In the **Drako sprite**:

```scratch
when I receive [showDrako v]
show
switch backdrop to [Inside Castle v]
say [Are you ready to feel my bite?] for 2 secs
ask [What is the spell?] and wait

if <(answer) = [luminos drakoria]> then
  say [Nooo! You have defeated me!] for 2 secs
  hide
  broadcast [victory v]
else
  say [Now you are my slave! Game over!] for 2 secs
  broadcast [defeat v]
end
```

---

### ⏱️ **25–45 min: Adding Win and Loss Logic**

**Optional: Add a backdrop for the ending** or switch to a "Victory" or "Game Over" screen

* Use `when I receive [victory]` or `[defeat]` to switch backdrops or show messages

```scratch
when I receive [victory v]
switch backdrop to [Victory v]

when I receive [defeat v]
switch backdrop to [Game Over v]
```

---

### **Differentiation:**

**💡 Less Confident:**

* Focus on copying basic blocks for scene switching and input checking
* Use one default spell hardcoded and one response (e.g. win or lose)

**✨ Average Confidence:**

* Complete full structure with both win and lose outcomes
* Add a backdrop change on `showDrako`
* Include correct positioning of sprites

**🚀 More Confident:**

* Add:

  * Sound effects
  * Custom animations (e.g. Drako shrinking, glowing spell effect)
  * Timers before transitions
  * A variable that tracks whether the spell was learned
  * A “Restart” button

---

### ⏱️ **45–55 min: Testing & Refining**

👾 Children test the full playthrough:

* Can the PC trigger the final scene?
* Does Drako appear properly?
* Are inputs correctly evaluated?
* Are win and lose endings working as intended?

✅ Encourage fixing logic bugs and making the transitions smooth.

---

### ⏱️ **55–60 min: Showcase & Celebration**

🎉 Children play each other’s games in pairs or small groups
🎤 Invite 2–3 children to screen-share and show their Drako battle

**Ask:**

* What was most fun about making this game?
* What would you add next?

---

## ✅ **By the end of Lesson 3, children will have...**

* Coded a complete beginning–middle–end structure
* Used broadcasts and inputs to trigger events
* Designed their own ending using conditional logic
* Created an interactive narrative RPG using foundational coding skills

---
