# ⚫ Stacks in Tech Interviews 2024: 21 Must-Know Questions & Answers

**Stacks** are linear data structures that follow the Last In, First Out (LIFO) principle, meaning the most recently added element is the first to be removed. They are foundational in tasks like parenthesis matching, undo operations, and depth-first search. In coding interviews, questions about stacks test a candidate's understanding of **sequential data storage** and its applications in various computational scenarios.

Check out our carefully selected list of **basic** and **advanced** Stacks questions and answers to be well-prepared for your tech interviews in 2024.

![Stacks Decorative Image](https://firebasestorage.googleapis.com/v0/b/dev-stack-app.appspot.com/o/blogImg%2Fstacks.png?alt=media&token=ec00727b-b6bc-4a03-a1b9-6d422bfa54e9&_gl=1*1mqplsu*_ga*OTYzMjY5NTkwLjE2ODg4NDM4Njg.*_ga_CW55HF8NVT*MTY5ODYwNTk1NS4xOTAuMS4xNjk4NjA2NzI0LjM2LjAuMA..)

👉🏼 You can also find all answers here: [Devinterview.io - Stacks](https://devinterview.io/data/stacks-interview-questions)

---

## 🔹 1. What is a _Stack_?

### Answer

A **stack** is a simple data structure that follows the **Last-In, First-Out (LIFO)** principle. It's akin to a stack of books, where the most recent addition is at the top and easily accessible.

### Core Characteristics

- **Data Representation**: Stacks can hold homogeneous or heterogeneous data.
- **Access Restrictions**: Restricted access primarily to the top of the stack, making it more efficient for certain algorithms.

### Stack Operations

1. **Push**: Adds an element to the top of the stack.
2. **Pop**: Removes and returns the top element.
3. **Peek**: Returns the top element without removing it.
4. **isEmpty**: Checks if the stack is empty.
5. **isFull** (for array-based stacks): Checks if the stack is full.

All the above operations typically have a time complexity of $O(1)$, making stack operations highly efficient.

### Visual Representation

![Stack Data Structure](https://firebasestorage.googleapis.com/v0/b/dev-stack-app.appspot.com/o/stacks%2Fstack.png?alt=media&token=74633f0a-83f7-4038-8b82-e10f0d6006b9&_gl=1*1uzhlk1*_ga*OTYzMjY5NTkwLjE2ODg4NDM4Njg.*_ga_CW55HF8NVT*MTY5NjYwNzMxNS4xNDcuMS4xNjk2NjA3NzE2LjUwLjAuMA..)

### Practical Applications

1. **Function Calls**: The call stack keeps track of program flow and memory allocation during method invocations.
2. **Text Editors**: The undo/redo functionality often uses a stack.
3. **Web Browsers**: The Back button's behavior can be implemented with a stack.
4. **Parsing**: Stacks can be used in language processing for functions like balanced parentheses, and **binary expression evaluation**.

5. **Memory Management**: Stacks play a role in managing dynamic memory in computer systems.

6. **Infix to Postfix Conversion**: It's a crucial step for evaluating mathematical expressions such as `2 + 3 * 5 - 4` in the correct precedence order. Stack-based conversion simplifies parsing and involves operators such as `push` and `pop` until the correct order is achieved.

7. **Graph Algorithms**: Graph traversal algorithms such as Depth First Search (DFS) deploy **stacks** as a key mechanism to remember vertices and explore connected components.

### Code Example: Basic Stack

Here is the Python code:

```python
class Stack:
    def __init__(self):
        self.stack = []

    def push(self, item):
        self.stack.append(item)

    def pop(self):
        if not self.is_empty():
            return self.stack.pop()

    def peek(self):
        if not self.is_empty():
            return self.stack[-1]

    def is_empty(self):
        return len(self.stack) == 0

    def size(self):
        return len(self.stack)
```

---

## 🔹 2. Why _Stack_ is considered a _Recursive_ data structure?

### Answer

A **stack** is considered a **recursive data structure** because its definition is self-referential. At any given point, a stack can be defined as a top element combined with another stack (the remainder).

Whenever an element is pushed onto or popped off a stack, what remains is still a stack. This **self-referential nature**, where operations reduce the problem to smaller instances of the same type, embodies the essence of **recursion**

---

## 🔹 3. When should I use _Stack_ or _Queue_ data structures instead of _Arrays/Lists_?

### Answer

**Queues** and **Stacks** provide structured ways to handle data, offering distinct advantages over more generic structures like **Lists** or **Arrays**.

### Key Features

#### Queues 

- **Characteristic**: First-In-First-Out (FIFO)
- **Usage**: Ideal for ordered processing, such as print queues or BFS traversal.

#### Stacks

- **Characteristic**: Last-In-First-Out (LIFO)
- **Usage**: Perfect for tasks requiring reverse order like undo actions or DFS traversal.

#### Lists/Arrays

- **Characteristic**: Random Access
- **Usage**: Suitable when you need random access to elements or don't require strict order or data management.

---

## 🔹 4. What are _Infix_, _Prefix_ and _Postfix_ notations?

### Answer

In computer science, **infix**, **prefix**, and **postfix** notations are methods of writing mathematical expressions. While humans generally use infix notation, machines can more efficiently parse prefix and postfix notations.

### Infix, Prefix and Postfix Notations

- **Infix**: Operators are placed between operands. This is the most common notation for humans due to its intuitiveness.
  
  Example: $1 + 2$

- **Prefix**: Operators are placed before operands. The order of operations is determined by the position of the operator rather than parentheses.
  
  Example: $+ 1 \times 2 3$ which evaluates to $1 + (2 \times 3) = 7$

- **Postfix**: Operators are placed after operands. The order of operations is determined by the sequence in which operands and operators appear.
  
  Example: $1 2 3 \times +$ which evaluates to $1 + (2 \times 3) = 7$

### Relation to Stacks

- **Conversion**: Stacks can facilitate the conversion of expressions from one notation to another. For instance, the Shunting Yard algorithm converts infix expressions to postfix notation using a stack.
  
- **Evaluation**: Both postfix and prefix expressions are evaluated using stacks. For postfix:
  1. Operands are pushed onto the stack.
  2. Upon encountering an operator, the required operands are popped, the operation is executed, and the result is pushed back.

  For example, for the expression $1 2 3 \times +$:
  - 1 is pushed onto the stack.
  - 2 is pushed.
  - 3 is pushed.
  - $\times$ is encountered. 3 and 2 are popped, multiplied to get 6, which is then pushed.
  - $+$ is encountered. 6 and 1 are popped, added to get 7, which is then pushed. This 7 is the result.

Evaluating prefix expressions follows a similar **stack-based method** but traverses the expression differently.

### Code Example: Postfix Evaluation

Here is the Python code:

```python
def evaluate_postfix(expression):
    stack = []
    tokens = expression.split()  # Handle multi-digit numbers
    for token in tokens:
        if token.isdigit():
            stack.append(int(token))
        else:
            operand2 = stack.pop()
            operand1 = stack.pop()
            stack.append(perform_operation(operand1, operand2, token))
    return stack[0]

def perform_operation(operand1, operand2, operator):
    operations = {
        '+': operand1 + operand2,
        '-': operand1 - operand2,
        '*': operand1 * operand2,
        '/': operand1 / operand2
    }
    return operations[operator]

# Example usage
print(evaluate_postfix('1 2 + 3 4 * -'))  # Output: -7
```

---

## 🔹 5. Compare _Array-based_ vs _Linked List_ stack implementations.

### Answer

**Array-based stacks** excel in time efficiency and direct element access. In contrast, **linked list stacks** are preferable for dynamic sizing and easy insertions or deletions.

### Common Features

- **Speed of Operations**: Both `pop` and `push` are $O(1)$ operations.
- **Memory Use**: Both have $O(n)$ space complexity.
- **Flexibility**: Both can adapt their sizes, but their resizing strategies differ.

### Key Distinctions

#### Array-Based Stack

- **Locality**: Consecutive memory locations benefit CPU caching.
- **Random Access**: Provides direct element access.
- **Iterator Needs**: Preferable if indexing or iterators are required.
- **Performance**: Slightly faster for top-element operations and potentially better for time-sensitive tasks due to caching.
- **Push**: $O(1)$ on average; resizing might cause occasional $O(n)$.

#### Linked List Stack

- **Memory Efficiency**: Better suited for fluctuating sizes and limited memory scenarios.
- **Resizing Overhead**: No resizing overheads.
- **Pointer Overhead**: Requires extra memory for storing pointers.

### Code Example: Array-Based Stack

Here is the Python code:

```python
class ArrayBasedStack:
    def __init__(self):
        self.stack = []
    def push(self, item):
        self.stack.append(item)
    def pop(self):
        return self.stack.pop() if self.stack else None
```

### Code Example: Linked List Stack

Here is the Python code:

```python
class Node:
    def __init__(self, data=None):
        self.data = data
        self.next = None
class LinkedListStack:
    def __init__(self):
        self.head = None
    def push(self, item):
        new_node = Node(item)
        new_node.next = self.head
        self.head = new_node
    def pop(self):
        if self.head:
            temp = self.head
            self.head = self.head.next
            return temp.data
        return None
```

---

## 🔹 6. Design a _Stack_ that supports _Retrieving_ the min element in _O(1)_.

### Answer

### Problem Statement

The goal is to design a **stack** data structure that can efficiently retrieve both the minimum element and the top element in $O(1)$ time complexity. 

### Solution

To meet the time complexity requirement, we'll maintain two stacks:

1. **Main Stack** for standard stack functionality.
2. **Auxiliary Stack** that keeps track of the minimum element up to a given stack position.

#### Algorithm Steps

1. **Pop** and **Push**
   - For each element $e$ in the **Main Stack**, check if it's smaller than or equal to the top element in the **Auxiliary Stack**. If $e$ is the new minimum, push it onto both stacks.

2. **Minimum Element Retrieval**: The top element of the **Auxiliary Stack** will always be the minimum element of the main stack.

#### Complexity Analysis

- **Time Complexity**: $O(1)$ for all operations.
- **Space Complexity**: $O(N)$, where $N$ is the number of elements in the stack.

#### Implementation

Here is the Python code:

```python
class MinStack:
    def __init__(self):
        self.stack = []
        self.min_stack = []

    def push(self, element):
        self.stack.append(element)
        if not self.min_stack or element <= self.min_stack[-1]:
            self.min_stack.append(element)

    def pop(self):
        if not self.stack:
            return None
        top = self.stack.pop()
        if top == self.min_stack[-1]:
            self.min_stack.pop()
        return top

    def top(self):
        return self.stack[-1] if self.stack else None

    def getMin(self):
        return self.min_stack[-1] if self.min_stack else None
```

---
## 🔹 7. Implement a _Linked List_ using _Stack_.

### Answer

👉🏼 Check out all 21 answers here: [Devinterview.io - Stacks](https://devinterview.io/data/stacks-interview-questions)

---

## 🔹 8. Implement Doubly Linked List using Stacks with min complexity.

### Answer

👉🏼 Check out all 21 answers here: [Devinterview.io - Stacks](https://devinterview.io/data/stacks-interview-questions)

---

## 🔹 9. Implement a _Queue_ using _Two Stacks_.

### Answer

👉🏼 Check out all 21 answers here: [Devinterview.io - Stacks](https://devinterview.io/data/stacks-interview-questions)

---

## 🔹 10. Implement a _Queue_ using only _One Stack_.

### Answer

👉🏼 Check out all 21 answers here: [Devinterview.io - Stacks](https://devinterview.io/data/stacks-interview-questions)

---

## 🔹 11. Implement _Stack_ using _Two Queues_ with efficient push.

### Answer

👉🏼 Check out all 21 answers here: [Devinterview.io - Stacks](https://devinterview.io/data/stacks-interview-questions)

---

## 🔹 12. Implement _Three Stacks_ with _One Array_.

### Answer

👉🏼 Check out all 21 answers here: [Devinterview.io - Stacks](https://devinterview.io/data/stacks-interview-questions)

---

## 🔹 13. _Reverse_ a _String_ using _Stack_.

### Answer

👉🏼 Check out all 21 answers here: [Devinterview.io - Stacks](https://devinterview.io/data/stacks-interview-questions)

---

## 🔹 14. _Reverse_ a _Stack_ without using any additional data structure.

### Answer

👉🏼 Check out all 21 answers here: [Devinterview.io - Stacks](https://devinterview.io/data/stacks-interview-questions)

---

## 🔹 15. _Sort_ a _Stack_ using _Recursion_.

### Answer

👉🏼 Check out all 21 answers here: [Devinterview.io - Stacks](https://devinterview.io/data/stacks-interview-questions)

---

## 🔹 16. _Sort_ a _Stack_ using another _Stack_.

### Answer

👉🏼 Check out all 21 answers here: [Devinterview.io - Stacks](https://devinterview.io/data/stacks-interview-questions)

---

## 🔹 17. _Check_ if parentheses are _Balanced_ using _Stack_.

### Answer

👉🏼 Check out all 21 answers here: [Devinterview.io - Stacks](https://devinterview.io/data/stacks-interview-questions)

---

## 🔹 18. _Find Duplicate Parenthesis_ in an expression.

### Answer

👉🏼 Check out all 21 answers here: [Devinterview.io - Stacks](https://devinterview.io/data/stacks-interview-questions)

---

## 🔹 19. Given an _Extremely Large File_ that doesn't fit into memory, check if the parentheses are _Balanced_.

### Answer

👉🏼 Check out all 21 answers here: [Devinterview.io - Stacks](https://devinterview.io/data/stacks-interview-questions)

---

## 🔹 20. Check for _Braces Balance_ in a really large (1T) file in _Parallel_.

### Answer

👉🏼 Check out all 21 answers here: [Devinterview.io - Stacks](https://devinterview.io/data/stacks-interview-questions)

---

## 🔹 21. Build a _Binary Expression Tree_ for the given expression.

### Answer

👉🏼 Check out all 21 answers here: [Devinterview.io - Stacks](https://devinterview.io/data/stacks-interview-questions)

---

