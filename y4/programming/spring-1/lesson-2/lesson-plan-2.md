# **Lesson 2: Coding Movement and NPC Interactions**

**Duration:** 60 minutes
**Lesson Focus:**

* Coding PC movement with `change x` and `change y`
* NPC riddle interactions triggered by touching the PC sprite
* Using `broadcast` and `when I receive` to control NPC appearances
* Creating simple input-checking logic with `if` and `else`

---

## **Learning Objectives:**

✅ Use Scratch to control sprite movement using arrow keys
✅ Detect collisions between the PC and an NPC
✅ Use `ask` blocks and `if` statements to evaluate riddle answers
✅ Use `broadcast` and `when I receive` to control visibility and game flow

---

## **Lesson Breakdown**

### ⏱️ **0–10 min: Recap & Hook – Revisit the World**

* Children open their Scratch projects from Lesson 1.
* Show the class a short demo of the finished interaction sequence:

  * Hero walks to NPC1 → asked a riddle → answers correctly → NPC2 appears.
  * If answer is wrong → no more NPCs appear → hero must visit Drako and fail.
* Explain today’s goal: *“You’ll bring your world to life with coding. The hero must meet each NPC, solve their riddle, and unlock the next step of the journey!”*

---

### Teaching Input (15 minutes)
Go over how to get the pc sprite to move and an example of how broadcast and when i receive message blocks work. Show the children how to get the pc and npc interaction working. If preferred the video in our shared area can be used :smiley:

---

### ⏱️ **10–20 min: Movement Code**

💻 *Focus: Getting the PC sprite to move*

* Children add arrow key controls using `when key pressed`, `change x`, and `change y`.

```scratch
when [right arrow] key pressed
change x by 5

when [left arrow] key pressed
change x by -5

when [up arrow] key pressed
change y by 5

when [down arrow] key pressed
change y by -5
```

**Differentiation:**

* 💡 *Less confident:* Copy pre-written movement code from a card or example.
* ✨ *Average:* Write all four directions independently.
* 🚀 *More confident:* Add animations (e.g. change costume while walking).

---

### ⏱️ **20–45 min: Coding NPC Interactions**

💡 *Focus: When the PC sprite touches the first NPC, a riddle is asked.*

**Step-by-step NPC 1 interaction:**

1. NPC 1 starts **visible**, NPC 2 and NPC 3 are **hidden**.
2. Use a loop to **check for touching the PC sprite**.
3. When touched, the NPC asks a riddle using the `ask` block.
4. If the answer is correct (checked with `if <answer = "x">`),

   * Broadcast `npc2-appear`,
   * Hide NPC 1.
5. If incorrect, nothing else happens.

```scratch
forever
  if <touching [PC sprite]> then
    ask [What has hands but cannot clap?] and wait
    if <(answer) = "clock"> then
      broadcast [npc2-appear v]
      hide
    end
  end
```

**For NPC 2 and NPC 3:**

* Start hidden.
* Use `when I receive [npc2-appear]` to show NPC 2, and so on.
* Structure is the same as NPC 1.

**Final broadcast from NPC 3:**

* Broadcast `spell-learned` when correct riddle is answered.
* Save spell in a **variable** (optional for confident children).

---

### **Differentiation for Coding NPCs:**

* 💡 *Less confident:* Work with a **guided template**, use fewer blocks, and only code NPC 1.
* ✨ *Average:* Code NPC 1, 2 and 3 with full interaction and broadcasts.
* 🚀 *More confident:*

  * Add a visual spell or message when all riddles are complete.

---

### ⏱️ **45–55 min: Testing & Refining**

🔁 Children test their projects:

* Can the hero move correctly?
* Does the first riddle appear?
* Does answering it correctly unlock the next NPC?
* If wrong, is the game stuck (as intended)?

🔧 Encourage them to fix any bugs or polish movement.

---

### ⏱️ **55–60 min: Plenary & Next Steps**

🧠 *Recap Key Concepts:*

* Movement with x and y
* `ask`, `if`, and `answer`
* `broadcast` and `when I receive`

🎯 *Preview of Lesson 3:*

* Next time we code the *final showdown with Drako*.
* Children will use the spell they learned to *win the game—or face defeat!*

---

## ✅ **Outcomes by End of Lesson 2:**

* PC sprite moves around the world
* First NPC asks a riddle and only progresses the story if answered correctly
* Broadcast messages control appearance of NPC 2 and 3
* Children understand input handling and simple control flow in Scratch

---
