### Lesson 1: Introduction to `str` and `int` Data Types in Python with Variables and String Concatenation

**Objective**:  
By the end of this lesson, students will understand how to work with `str` (string) and `int` (integer) data types, how to create variables in Python, how to cast an integer to a string, and how to concatenate strings. This lesson is designed as an introduction to Python programming using [trinket](https://trinket.io/python3) preparing them for later lessons where they will use these concepts on the micro:bit.

---

### Lesson Outline (60 Minutes)

---

**1. Review and Warm-Up (5 minutes)**

- **Objective**: Recap any basic programming knowledge from previous lessons (e.g., what variables are, how they store values) and set the stage for the lesson on data types.
- **Discussion**: Review how data are stored in variables | Scratch can be used for this or a physical demonstration can be given using containers and slips of paper with values on them.

---

**2. Teaching Input | Introducing Data Types: `str` and `int` (5 minutes)**

- **Explanation**:
  - **Data Types in Python**: Introduce the concept of data types. Explain that Python can handle different types of data:
    - **`str` (String)**: A sequence of characters enclosed in quotes. Example: `"Alice"`, `"Hello"`, `"1234"`.
    - **`int` (Integer)**: A whole number, which can be positive or negative. Example: `5`, `-7`, `23`.
  - **Variables**: Show how variables store data of a specific type. Example: 
    ```python
    name = "Alice"  # This is a string variable
    age = 11        # This is an integer variable
    ```

- **Example**:
    - Declare two variables: `name` (string) and `age` (integer).
    - Print out a greeting message that uses these variables.
    ```python
    name = "Alice"
    age = 11
    print(name)
    print(age)
    ```

---

**3. Working with Variables and String Concatenation (5 minutes)**

- **Explanation**:
  - **String Concatenation**: Teach how to combine strings using the `+` operator.
  - **Casting an Integer to a String**: Explain how to convert an integer into a string using `str()`. This is important when you want to concatenate numbers with strings.

- **Example**:
  - Concatenate strings and numbers by casting the integer to a string:
    ```python
    name = "Alice"
    age = 11
    greeting = "Hello, " + name + ". You are " + str(age) + " years old."
    print(greeting)
    ```
>[!NOTE]
>The video in our shared area can be used to teach the above points if not feeling confident :smiley:

---

**4. Hands-On Practice (40 minutes)**

- **Exercise 1**: 
  - **Task**: Write a Python program where the name and age are hardcoded, and the program outputs a sentence with the person’s name and age using string concatenation.
  - Example output:  
    `"Hello, Alice! You are 11 years old."`
  
  - **Instructions**:
    1. Create two variables: `name` and `age`.
    2. Use string concatenation to form a complete sentence and print it.

- **Exercise 2**: 
  - **Task**: Modify the program to include a favorite color.
  - Example output:  
    `"Hello, Alice! You are 11 years old and your favorite color is blue."`
  
  - **Instructions**:
    1. Add a `color` variable.
    2. Modify the greeting message to include the favorite color using concatenation.

- **Projects**:
  - The children could work on a project instead of the above exercises - if they feel more confident - or they could do so after trying the exercises if they prefer.
  - Please see [projects](projects.md) for ideas.

---

**5. Recap and Q&A (5 minutes)**

- **Objective**: Review the key concepts of the lesson: data types, variables, string concatenation, and casting between data types.
- **Key Points to Review**:
  - What is the difference between `str` and `int` data types?
  - How do we concatenate strings?
  - How do we cast an integer to a string using `str()`?

---

### Example Code for the Lesson:

```python
# Part 1: Introduction to variables and data types
name = "Alice"
age = 11

# Part 2: String concatenation
greeting = "Hello, " + name + ". You are " + str(age) + " years old."
print(greeting)

# Part 3: Add a favorite color
color = "blue"
favorite_color_message = "Hello, " + name + ". You are " + str(age) + " years old and your favorite color is " + color + "."
print(favorite_color_message)
```

---

### Differentiation:

- **Less Confident Programmers**: Focus on achieving the exercises with the support of watching and pausing the teaching video if needed.
- **Average Confidence Programmers**: Get them to solve one or more of the example [projects](projects.md) after completing the exercises.
- **More Confident Programmers**: Challenge them to solve one or more of the example [projects](projects.md) without working on the exercises.

---

This lesson will give students a solid foundation in Python data types and string manipulation, preparing them for more complex projects that will involve the micro:bit in subsequent lessons.
