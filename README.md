# Python Assignment 2 – Data Structures: List, Dictionary, Set & Conditional Statements

## Assignment Overview

This assignment demonstrates the use of Python Lists, Dictionaries, Sets, and Conditional Statements. The following tasks were completed step by step using Python and Jupyter Notebook.

---

# 1. LIST

## 1. Create a list called `age_list` with five integers.

    age_list = [21, 22, 23, 24, 25]

## 2. Create a list called `name_list` with five strings.

    name_list = ["Rahul", "Arjun", "Neha", "Sneha", "Akhil"]

## 3. Append `"Yazhini"` to `name_list`.

    name_list.append("Yazhini")

    Output:
    ['Rahul', 'Arjun', 'Neha', 'Sneha', 'Akhil', 'Yazhini']

## 4. Insert `30` at index `2` in `age_list`.

    age_list.insert(2, 30)

    Output:
    [21, 22, 30, 23, 24, 25]

## 5. Remove `"Yazhini"` from `name_list`.

    name_list.remove("Yazhini")

    Output:
    ['Rahul', 'Arjun', 'Neha', 'Sneha', 'Akhil']

## 6. Pop the last element from `age_list`.

    age_list.pop()

    Output:
    25

## 7. Extend `age_list` with `[29, 30, 26]`.

    age_list.extend([29, 30, 26])

    Output:
    [21, 22, 30, 23, 24, 29, 30, 26]

## 8. Sort `age_list` in descending order.

    age_list.sort(reverse=True)

    Output:
    [30, 30, 29, 26, 24, 23, 22, 21]

## 9. Find the maximum, minimum, and sum of `age_list`.

    max(age_list)

    Output:
    30

    min(age_list)

    Output:
    21

    sum(age_list)

    Output:
    205

## 10. Access the first name, last name, indexes 2–4, and reverse `name_list`.

### First name

    print(name_list[0])

    Output:
    Rahul

### Last name

    print(name_list[-1])

    Output:
    Akhil

### Indexes 2–4

    print(name_list[2:5])

    Output:
    ['Neha', 'Sneha', 'Akhil']

### Reverse the list

    print(name_list[::-1])

    Output:
    ['Akhil', 'Sneha', 'Neha', 'Arjun', 'Rahul']

---

# 2. DICTIONARY

## a. Create `student_marks` mapping five students to marks from 0–100.

    student_marks = {
        "Rahul": 76,
        "Arjun": 89,
        "Neha": 91,
        "Sneha": 78,
        "Akhil": 84
    }

## b. Print the mark of a specific student.

    print(student_marks["Neha"])

    Output:
    91

## c. Add `Janani: 80`.

    student_marks["Janani"] = 80

    Output:
    {'Rahul': 76, 'Arjun': 89, 'Neha': 91, 'Sneha': 78, 'Akhil': 84, 'Janani': 80}

## d. Update any older student to `82`.

    student_marks["Rahul"] = 82

    Output:
    {'Rahul': 82, 'Arjun': 89, 'Neha': 91, 'Sneha': 78, 'Akhil': 84, 'Janani': 80}

## e. Use `keys()`, `values()`, and `items()` to print all.

### keys()

    print(student_marks.keys())

    Output:
    dict_keys(['Rahul', 'Arjun', 'Neha', 'Sneha', 'Akhil', 'Janani'])

### values()

    print(student_marks.values())

    Output:
    dict_values([82, 89, 91, 78, 84, 80])

### items()

    print(student_marks.items())

    Output:
    dict_items([('Rahul', 82), ('Arjun', 89), ('Neha', 91), ('Sneha', 78), ('Akhil', 84), ('Janani', 80)])

---

# 3. SETS

## a. Create `my_set` from `['a','e','i','o','u','a','a','i']`. Analyze the duplicate output.

    my_set = {'a', 'e', 'i', 'o', 'u', 'a', 'a', 'i'}
    print(my_set)

    Output:
    {'a', 'e', 'i', 'o', 'u'}

### Explanation

A Set does not allow duplicate elements. Therefore, the repeated values `'a'` and `'i'` appear only once in the output.

## b. Attempt `my_set[4] = 's'`. If there is an error, explain.

    my_set[4] = 's'

    Output:
    TypeError: 'set' object does not support item assignment

### Explanation

Sets are unordered collections and do not support indexing or item assignment. Therefore, an element cannot be changed using an index.

## c. Create `set1` and `set2`.

    set1 = {1, 3, 5, 7, 9}
    set2 = {2, 3, 5, 8, 10}

## d. Print the union and intersection.

### Union

    print(set1.union(set2))

    Output:
    {1, 2, 3, 5, 7, 8, 9, 10}

### Intersection

    print(set1.intersection(set2))

    Output:
    {3, 5}

---

# 4. CONDITIONAL STATEMENTS

## Score: 0–10 inclusive

The score is categorized using the following conditions:

- Above Average: Score greater than 7
- Average: Score from 4 to 7 inclusive
- Below Average: Score less than 4

## Python Code

    score = int(input("Enter your score (0 to 10): "))

    if score > 7:
        print("Above Average: Excellent performance! Keep up the great work.")
    elif score >= 4:
        print("Average: Good effort! Keep practicing, there's room for improvement.")
    else:
        print("Below Average: Need to improve your performance. Consistent practice will lead to better results.")

## Sample Input

    Enter your score (0 to 10): 7

## Output

    Average: Good effort! Keep practicing, there's room for improvement.

---

# CONCLUSION

This assignment provided practical experience with Python Lists, Dictionaries, Sets, and Conditional Statements. The exercises covered creating and modifying data structures, accessing and manipulating elements, performing mathematical and set operations, handling duplicate values, understanding Set immutability, and using IF, ELIF, and ELSE statements for decision-making based on user input.

## Tools Used

- Python
- Jupyter Notebook

## Project File

Python_Assignment_2_Data_Structures.ipynb
