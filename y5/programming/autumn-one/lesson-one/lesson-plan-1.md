### Lesson 1: Introduction to the Space Game and Using OR Logic

**Objective**: Introduce the Space Game project, basic spaceship movement, and collecting items with OR logic.

#### 1. Introduction and Review (10 minutes)
- Review `broadcast message` and `when i receive message` using [review activities](review.md)
- Explain the project for this first lesson: controlling a spaceship to collect items and pass through a portal to finish the game.
- Introduce the concept of OR logic using simple examples...
##### Boolean OR Logic:
1. **Explanation**:
   - Let's say you have two different types of sweet: chocolate and gummy bears.
   - Your mom says, "You can have a treat if you have a chocolate OR a gummy bear."
   - In this situation, if you have a chocolate, we say that having chocolate is **true**. If you don't have a chocolate, it's **false**.
   - If you have a gummy bear, we say that having a gummy bear is **true**. If you don't have a gummy bear, it's **false**.
   - To get a treat, either one of these needs to be **true** (chocolate **true** OR gummy bear **true**).

2. **Scratch Example**:
   - In Scratch, OR logic is used to check if at least one condition is **true**.
   - If your spaceship needs to collect a red crystal OR a blue crystal to go through the portal, the game will check if having a red crystal is **true** OR having a blue crystal is **true**.
   - You can go through the portal if either one is **true**.

###### Activities to Help Understand:
- **OR Logic**: 
  - Ask the children to stand up if they like apples OR bananas.
  - Explain that if they like apples (apples **true**) OR if they like bananas (bananas **true**), they stand up. If they like both, they still stand up.

#### 2. Modelled Example (20 minutes)
- Model how to create the simple project.
- Add a spaceship sprite and a space background.
- Show how to use the `move` and `point in direction` blocks to control the spaceship with arrow keys.
- Add red and blue crystal sprites.
- Show how to use a `wait until` statement to check if the spaceship is touching a crystal.
- Variables can be used to keep track of whether or not a red crystal or a blue crystal have been collected.
- Show how the portal sprite will only broadcast a gameOver message if a red crystal `or` a blue crystal has been collected.
- Use `broadcast message` and `when i receive message` blocks to switch the backdrop to a game over one.
- If not confident with the above please use the video in our shared area 😃

#### 3. Programming Time (30 minutes)
- The children now program and get their projects working

#### 4. Differentiation
- **Less Confident Programmers**: 
  - Provide screenshots and focus on getting the `or` logic to work | the crystals could just stay in one place.
- **Average Programmers**: 
  - Encourage them to get the crystals to move to random positions.
- **More Confident Programmers**: 
  - Challenge them to add more items to collect and use OR logic to check for multiple items | maybe different coloured crystals.
  - Challenge them to use a sequence of `if` blocks to trigger different game over backdrops based on the items collected.

