# ☀️ Weather Wizards - The Python Edition ☀️

---

## **Lesson 2: Reading and Displaying Temperature on a Micro:bit**  
#### **Objective:**  
Children will build on their knowledge of `str`, `int`, and `print()` by coding a virtual micro:bit to read and display the temperature. They will use `display.scroll()` to output the temperature as a string.  

---  

## **Lesson Structure (60 Minutes)**  

### **1️⃣ Review Activity (5 Minutes) – Off-Computer**  
📢 **Quick Review Game: "Code Translator"**  

- Write these **Python expressions** on the board:  
  1. `temperature = 20`  
  2. `print("The temperature is " + temperature + " C")`  
  3. `print("The temperature is " + str(temperature) + " C")`  

**Task:**  
- Ask the children **why line 2 will cause an error** and what needs to be fixed.  
- They should recognize that `temperature` is an `int` and must be **cast** to `str`.  
- Use an analogy: **"You can't glue numbers to words unless you change the numbers into words first!"**  

---  

### **2️⃣ Introduction (10 Minutes) – Linking to Previous Learning**  
1. **Why We’re Using `display.scroll()` Instead of `print()`**  
   - In Trinket, we used `print()` to send messages to the terminal.  
   - On a micro:bit, there’s no screen like Trinket, so we use **`display.scroll()`** to show text.  

2. **How Sensors Work in Python**  
   - The micro:bit has a built-in **temperature sensor** that gives an `int` value.  
   - We need to **cast** it to `str` to display it!  

---  

### **3️⃣ Main Task (30 Minutes) – Coding the Temperature Reader**  

>[!NOTE]
>The video in our shared area can be used to demonstrate how to code this along with explanations 😃

**Task:** Write a program in the [official micro:bit Python online editor](https://python.microbit.org/v/3) to:  
1. Read the **temperature** using `temperature()`.  
2. Convert it to **str**.  
3. Use `display.scroll()` to show it on the micro:bit screen.  
4. Make it repeat every 5 seconds using `while True:` and `sleep(5000)`.  

💻 **Starter Code for All Learners:**  
```python
from microbit import *

while True:
    temp = temperature()  # Get temperature as an int
    temp_to_string = str(temp) # Cast int to str
    display.scroll("Temp: " + temp_to_string)  # Display the value
    sleep(5000)  # Wait 5 seconds
```

---

### **4️⃣ Differentiation & Challenges**  

#### 🔹 **Less Confident Coders:**  
- Can watch the video and code along with it  

#### 🔸 **Average Coders:**  
- Once their temperature code is working, challenge them to **add light level**:  
  ```python
  light = display.read_light_level()
  ```
- Modify the program to **scroll both** temperature and light level in a loop.  

#### 🔺 **More Confident Coders:**   
- Try **using button A** to show only temperature and **button B** to show light level.
- Watch the extension video in the shared area to better understand what is happening under the hood

---

### **5️⃣ Wrap-Up & Reflection (10 Minutes)**  
📢 **Discussion Questions:**  
1. How is `display.scroll()` similar to `print()`?  
2. Why do we need to **cast** the temperature to `str`?  
3. What does `while True:` do in our program?  

✏️ **Exit Ticket:**  
- Ask them to **say one new thing** they learned today.  

---

### **Extra Challenge**  
- Bonus Task: Add a **custom message** for different temperature ranges (e.g., "Too hot!", "Just right!").  
