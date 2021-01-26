<div data-v-5e9078c0=""><h1 data-v-5e9078c0="">
      Top 25 Stacks interview
      questions and answers in 2021.
    </h1> <p data-v-5e9078c0="" align="center"><a data-v-5e9078c0="" href="https://devinterview.io/"><img data-v-5e9078c0="" src="https://source.unsplash.com/collection/52661698/700x350"></a></p> <p data-v-5e9078c0="">
      You can check all
      25
      Stacks interview questions here 👉
      https://devinterview.io/data/stacks-interview-questions
    </p> <br data-v-5e9078c0=""> 
    <div>

## 🔹 1\. Explain why Stack is a recursive data structure

</div>

<div>

### Answer:

<div class="answer">

<div>

<div>

<div class="AnswerBody">

A **stack** is a **recursive** data structure, so it's:

*   a stack is either empty or
*   it consists of a top and the rest which is a stack by itself;

</div>

</div>

<div class="row my-2">

<div><span>Source: <span>www.cs.cmu.edu https://www.cs.cmu.edu/~adamchik/15-121/lectures/Stacks%20and%20Queues/Stacks%20and%20Queues.html "Explain why Stack is a recursive data structure Interview Questions Source To Answer"</span></span>   </div>

</div>

</div>

</div>

</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 2\. Define Stack

</div>

<div>

### Answer:

<div class="answer">

<div>

<div>

<div class="AnswerBody">

A **Stack** is a container of objects that are inserted and removed according to the last-in first-out (**LIFO**) principle. In the pushdown stacks only two operations are allowed: push the item into the stack, and pop the item out of the stack.

There are basically three operations that can be performed on stacks. They are:

1.  inserting an item into a stack (**push**).
2.  deleting an item from the stack (**pop**).
3.  displaying the contents of the stack (**peek** or **top**).

A stack is a limited access data structure - elements can be added and removed from the stack only at the top. push adds an item to the top of the stack, pop removes the item from the top. A helpful analogy is to think of a stack of books; you can remove only the top book, also you can add a new book on the top.

</div>

</div>

<div class="row my-2">

<div><span>Source: <span>www.cs.cmu.edu https://www.cs.cmu.edu/~adamchik/15-121/lectures/Stacks%20and%20Queues/Stacks%20and%20Queues.html "Define Stack Interview Questions Source To Answer"</span></span>   </div>

</div>

</div>

</div>

</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 3\. Why and when should I use Stack or Queue data structures instead of Arrays/Lists?

</div>

<div>

### Answer:

<div class="answer">

<div>

<div>

<div class="AnswerBody">

Because they help manage your data in more a _particular_ way than arrays and lists. It means that when you're debugging a problem, you won't have to wonder if someone randomly inserted an element into the middle of your list, messing up some invariants.

Arrays and lists are random access. They are very flexible and also easily _corruptible_. If you want to manage your data as FIFO or LIFO it's best to use those, already implemented, collections.

More practically you should:

*   Use a queue when you want to get things out in the order that you put them in (FIFO)
*   Use a stack when you want to get things out in the reverse order than you put them in (LIFO)
*   Use a list when you want to get anything out, regardless of when you put them in (and when you don't want them to automatically be removed).

</div>

</div>

<div class="row my-2">

<div><span>Source: <span>stackoverflow.com https://stackoverflow.com/questions/2074970/stack-and-queue-why "Why and when should I use Stack or Queue data structures instead of Arrays/Lists? Interview Questions Source To Answer"</span></span>   </div>

</div>

</div>

</div>

</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 4\. Why Are Stacks Useful?

</div>

<div>

### Answer:

<div class="answer">

<div>

<div>

<div class="AnswerBody">

They’re very useful because they afford you constant time `_O_(_1_)` operations when _inserting_ or _removing_ from the front of a data structure. One common use of a stack is in compilers, where a stack can be used to make sure that the brackets and parentheses in a code file are all balanced, i.e., have an opening and closing counterpart. Stacks are also very useful in evaluating mathematical expressions.

</div>

</div>

<div class="row my-2">

<div><span>Source: <span>medium.com https://medium.com/better-programming/solving-the-min-stack-problem-in-o-1-time-using-a-single-stack-in-ruby-626f65142927 "Why Are Stacks Useful? Interview Questions Source To Answer"</span></span>   </div>

</div>

</div>

</div>

</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 5\. How to implement Linked List Using Stack?

</div>

<div>

### Answer:

<div class="answer">

<div>

<div>

<div class="AnswerBody">

You can simulate a linked list by using two stacks. One stack is the "list," and the other is used for temporary storage.

*   To **add** an item at the head, simply push the item onto the stack.
*   To **remove** from the head, pop from the stack.
*   To **insert** into the middle somewhere, pop items from the "list" stack and push them onto the temporary stack until you get to your insertion point. Push the new item onto the "list" stack, then pop from the temporary stack and push back onto the "list" stack. Deletion of an arbitrary node is similar.

This isn't terribly efficient, by the way, but it would in fact work.

</div>

</div>

<div class="row my-2">

<div><span>Source: <span>stackoverflow.com https://stackoverflow.com/questions/36150565/how-to-implement-linked-list-using-stack "How to implement Linked List Using Stack? Interview Questions Source To Answer"</span></span>   </div>

</div>

</div>

</div>

</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 6\. Implement a Queue using two Stacks

</div>

<div>

### Answer:

<div class="answer">

<div>

<div class="mb-2"><span class="h5">Problem</span></div>

<div>

<div class="AnswerBody">

Suppose we have two stacks and no other temporary variable. Is to possible to "construct" a queue data structure using only the two stacks?

</div>

</div>

<div>

<div class="AnswerBody">

Keep two stacks, let's call them `inbox` and `outbox`.

**Enqueue**:

*   Push the new element onto `inbox`

**Dequeue**:

*   If `outbox` is empty, refill it by popping **each** element from `inbox` and pushing it onto `outbox`
*   Pop and return the top element from `outbox`

</div>

</div>

<div>

<div class="mb-2 mt-2"><span class="h5">Complexity Analysis</span></div>

<div class="hide-small">

<div class="row no-gutters my-2 align-items-end">

<div class="col font-weight-bold text-muted">Time:</div>

<div class="col text-center">

<div class="text-muted font-weight-bold justify-content-center">Constant</div>

<div class="complexity amazing first p-1 justify-content-center shadow-text selected-complexity effect7">O(1)</div>

</div>

<div class="col disable text-center">

<div class="text-muted font-weight-bold justify-content-center">Dbl. Logarithmic</div>

<div class="complexity good p-1 justify-content-center shadow-text">O(log log n)</div>

</div>

<div class="col disable text-center">

<div class="text-muted font-weight-bold justify-content-center">Logarithmic</div>

<div class="complexity good p-1 justify-content-center shadow-text">O(log n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold  text-muted justify-content-center">Square Root</div>

<div class="complexity fair p-1 justify-content-center shadow-text ">O(√n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold  text-muted justify-content-center">Linear</div>

<div class="complexity fair p-1 justify-content-center shadow-text ">O(n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold text-muted justify-content-center">Linearithmic</div>

<div class="complexity bad p-1 justify-content-center shadow-text ">O(n log n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold  text-muted justify-content-center">Quadratic</div>

<div class="complexity terrible p-1 justify-content-center shadow-text ">_O_(_n_<sup>2</sup>)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold   text-muted justify-content-center">Exponential</div>

<div class="complexity terrible p-1 justify-content-center shadow-text ">_O_(_2_<sup>n</sup>)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold text-muted">Factorial</div>

<div class="complexity terrible last p-1 justify-content-center shadow-text ">O(n!)</div>

</div>

</div>

</div>

<div class="hide-small">

<div class="row no-gutters my-2 align-items-end">

<div class="col font-weight-bold text-muted">Space:</div>

<div class="col text-center">

<div class="text-muted font-weight-bold justify-content-center">Constant</div>

<div class="complexity amazing first p-1 justify-content-center shadow-text selected-complexity effect7">O(1)</div>

</div>

<div class="col disable text-center">

<div class="text-muted font-weight-bold justify-content-center">Dbl. Logarithmic</div>

<div class="complexity good p-1 justify-content-center shadow-text">O(log log n)</div>

</div>

<div class="col disable text-center">

<div class="text-muted font-weight-bold justify-content-center">Logarithmic</div>

<div class="complexity good p-1 justify-content-center shadow-text">O(log n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold  text-muted justify-content-center">Square Root</div>

<div class="complexity fair p-1 justify-content-center shadow-text ">O(√n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold  text-muted justify-content-center">Linear</div>

<div class="complexity fair p-1 justify-content-center shadow-text ">O(n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold text-muted justify-content-center">Linearithmic</div>

<div class="complexity bad p-1 justify-content-center shadow-text ">O(n log n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold   text-muted justify-content-center">Quadratic</div>

<div class="complexity terrible p-1 justify-content-center shadow-text ">_O_(_n_<sup>2</sup>)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold   text-muted justify-content-center">Exponential</div>

<div class="complexity terrible p-1 justify-content-center shadow-text ">_O_(_2_<sup>n</sup>)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold text-muted">Factorial</div>

<div class="complexity terrible last p-1 justify-content-center shadow-text ">O(n!)</div>

</div>

</div>

</div>

<div class="hide-large">

**Time:** <mark>O(1)</mark>

**Space:** <mark>O(1)</mark>

</div>

<div class="mt-3">

<div>

<div class="AnswerBody">

In the worst case scenario when outbox stack is empty, the algorithm pops n elements from inbox stack and pushes n elements to outbox, where n is the queue size. This gives `2*n` operations, which is `O(n)`. But when outbox stack is not empty the algorithm has `O(1)` time complexity that gives amortised `O(1)`.

</div>

</div>

</div>

</div>

<div style="font-size: 14px;">

<div class="mb-3 mt-2"><span class="h5">Implementation</span></div>

<div>

<nav class="mdc-tab-bar">

<div class="mdc-tab-scroller">

<div class="mdc-tab-scroller__scroll-area mdc-tab-scroller__scroll-area--scroll" style="margin-bottom: 0px;">

<div class="mdc-tab-scroller__scroll-content"><button class="mdc-ripple-upgraded mdc-ripple-upgraded--background-focused mdc-tab mdc-tab--min-width mdc-tab--active" aria-selected="true" tabindex="0">

<div class="mdc-tab__content"><span class="mdc-tab__text-label"><span>C#</span> <span class="shadow-text lang-badge cs">CS</span></span></div>

<span class="mdc-tab-indicator mdc-tab-indicator--active"><span aria-hidden="true" class="mdc-tab-indicator__content mdc-tab-indicator__content--underline"></span></span></button><button class="mdc-ripple-upgraded mdc-tab mdc-tab--min-width">

<div class="mdc-tab__content"><span class="mdc-tab__text-label"><span>JavaScript</span> <span class="shadow-text lang-badge js">JS</span></span></div>

<span class="mdc-tab-indicator"><span aria-hidden="true" class="mdc-tab-indicator__content mdc-tab-indicator__content--underline"></span></span></button><button class="mdc-ripple-upgraded mdc-tab mdc-tab--min-width">

<div class="mdc-tab__content"><span class="mdc-tab__text-label"><span>Java</span> <span class="shadow-text lang-badge java">Java</span></span></div>

<span class="mdc-tab-indicator"><span aria-hidden="true" class="mdc-tab-indicator__content mdc-tab-indicator__content--underline"></span></span></button><button class="mdc-ripple-upgraded mdc-tab mdc-tab--min-width">

<div class="mdc-tab__content"><span class="mdc-tab__text-label"><span>Python</span> <span class="shadow-text lang-badge py">PY</span></span></div>

<span class="mdc-tab-indicator"><span aria-hidden="true" class="mdc-tab-indicator__content mdc-tab-indicator__content--underline"></span></span></button></div>

</div>

</div>

</nav>

</div>

<div class="mt-2">

<div class="AnswerBody">

    public class Queue<T> where T : class
    {
        private Stack<T> input = new Stack<T>();
        private Stack<T> output = new Stack<T>();

        public void Enqueue(T t)
        {
            input.Push(t);
        }

        public T Dequeue()
        {
            if (output.Count == 0)
            {
                while (input.Count != 0)
                {
                    output.Push(input.Pop());
                }
            }

            return output.Pop();
        }
    }

</div>

</div>

</div>

<div class="row my-2">

<div><span>Source: <span>stackoverflow.com https://stackoverflow.com/questions/69192/how-to-implement-a-queue-using-two-stacks "Implement a Queue using two Stacks Interview Questions Source To Answer"</span></span>   </div>

</div>

</div>

</div>

</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 7\. Implement Stack using Two Queues (with efficient push)

</div>

<div>

### Answer:

<div class="answer">

<div>

<div class="mb-2"><span class="h5">Problem</span></div>

<div>

<div class="AnswerBody">

Given two queues with their standard operations (`enqueue`, `dequeue`, `isempty`, `size`), implement a stack with its standard operations (`pop`, `push`, `isempty`, `size`). The stack should be efficient when pushing an item.

</div>

</div>

<div>

<div class="AnswerBody">

Given we have `queue1` and `queue2`:

**push** - `O(1)`:

*   enqueue in `queue1`

**pop** - `O(n)`:

*   while size of `queue1` is bigger than 1, pipe (dequeue + enqueue) dequeued items from `queue1` into `queue2`
*   dequeue and return the last item of `queue1`, then switch the names of `queue1` and `queue2`

</div>

</div>

<div>

<div class="mb-2 mt-2"><span class="h5">Complexity Analysis</span></div>

<div class="hide-small">

<div class="row no-gutters my-2 align-items-end">

<div class="col font-weight-bold text-muted">Time:</div>

<div class="col text-center">

<div class="text-muted font-weight-bold justify-content-center">Constant</div>

<div class="complexity amazing first p-1 justify-content-center shadow-text selected-complexity effect7">O(1)</div>

</div>

<div class="col disable text-center">

<div class="text-muted font-weight-bold justify-content-center">Dbl. Logarithmic</div>

<div class="complexity good p-1 justify-content-center shadow-text">O(log log n)</div>

</div>

<div class="col disable text-center">

<div class="text-muted font-weight-bold justify-content-center">Logarithmic</div>

<div class="complexity good p-1 justify-content-center shadow-text">O(log n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold  text-muted justify-content-center">Square Root</div>

<div class="complexity fair p-1 justify-content-center shadow-text ">O(√n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold  text-muted justify-content-center">Linear</div>

<div class="complexity fair p-1 justify-content-center shadow-text ">O(n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold text-muted justify-content-center">Linearithmic</div>

<div class="complexity bad p-1 justify-content-center shadow-text ">O(n log n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold  text-muted justify-content-center">Quadratic</div>

<div class="complexity terrible p-1 justify-content-center shadow-text ">_O_(_n_<sup>2</sup>)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold   text-muted justify-content-center">Exponential</div>

<div class="complexity terrible p-1 justify-content-center shadow-text ">_O_(_2_<sup>n</sup>)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold text-muted">Factorial</div>

<div class="complexity terrible last p-1 justify-content-center shadow-text ">O(n!)</div>

</div>

</div>

</div>

<div class="hide-small">

<div class="row no-gutters my-2 align-items-end">

<div class="col font-weight-bold text-muted">Space:</div>

<div class="col text-center">

<div class="text-muted font-weight-bold justify-content-center">Constant</div>

<div class="complexity amazing first p-1 justify-content-center shadow-text selected-complexity effect7">O(1)</div>

</div>

<div class="col disable text-center">

<div class="text-muted font-weight-bold justify-content-center">Dbl. Logarithmic</div>

<div class="complexity good p-1 justify-content-center shadow-text">O(log log n)</div>

</div>

<div class="col disable text-center">

<div class="text-muted font-weight-bold justify-content-center">Logarithmic</div>

<div class="complexity good p-1 justify-content-center shadow-text">O(log n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold  text-muted justify-content-center">Square Root</div>

<div class="complexity fair p-1 justify-content-center shadow-text ">O(√n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold  text-muted justify-content-center">Linear</div>

<div class="complexity fair p-1 justify-content-center shadow-text ">O(n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold text-muted justify-content-center">Linearithmic</div>

<div class="complexity bad p-1 justify-content-center shadow-text ">O(n log n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold   text-muted justify-content-center">Quadratic</div>

<div class="complexity terrible p-1 justify-content-center shadow-text ">_O_(_n_<sup>2</sup>)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold   text-muted justify-content-center">Exponential</div>

<div class="complexity terrible p-1 justify-content-center shadow-text ">_O_(_2_<sup>n</sup>)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold text-muted">Factorial</div>

<div class="complexity terrible last p-1 justify-content-center shadow-text ">O(n!)</div>

</div>

</div>

</div>

<div class="hide-large">

**Time:** <mark>O(1)</mark>

**Space:** <mark>O(1)</mark>

</div>

<div class="mt-3">

<div>

<div class="AnswerBody">

If queue is implemented as _linked list_ the `enqueue` operation has `O(1)` time complexity.

</div>

</div>

</div>

</div>

<div style="font-size: 14px;">

<div class="mb-3 mt-2"><span class="h5">Implementation</span></div>

<div>

<nav class="mdc-tab-bar">

<div class="mdc-tab-scroller">

<div class="mdc-tab-scroller__scroll-area mdc-tab-scroller__scroll-area--scroll" style="margin-bottom: 0px;">

<div class="mdc-tab-scroller__scroll-content"><button class="mdc-ripple-upgraded mdc-ripple-upgraded--background-focused mdc-tab mdc-tab--min-width mdc-tab--active" aria-selected="true" tabindex="0">

<div class="mdc-tab__content"><span class="mdc-tab__text-label"><span>Java</span> <span class="shadow-text lang-badge java">Java</span></span></div>

<span class="mdc-tab-indicator mdc-tab-indicator--active"><span aria-hidden="true" class="mdc-tab-indicator__content mdc-tab-indicator__content--underline"></span></span></button></div>

</div>

</div>

</nav>

</div>

<div class="mt-2">

<div class="AnswerBody">

    public Stack<E> {
        private Queue<E> q1 = new Queue<E>();
        private Queue<E> q2 = new Queue<E>();

        public void push(E x) {
            q1.enqueue(x);
        }

        public E pop() {
            while (q1.size() > 1) {
                q2.enqueue(q1.dequeue());
            }
            E pop = q1.dequeue();
            Queue<E> temp = q1;
            q1 = q2;
            q2 = temp;
            return pop;
        }
    }

</div>

</div>

</div>

<div class="row my-2">

<div><span>Source: <span>stackoverflow.com https://stackoverflow.com/questions/688276/implement-stack-using-two-queues "Implement Stack using Two Queues (with efficient `push`) Interview Questions Source To Answer"</span></span>   </div>

</div>

</div>

</div>

</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 8\. What is complexity of push and pop for a Stack implemented using a LinkedList?

</div>

<div>

### Answer:

<div class="answer">

<div>

<div>

<div class="AnswerBody">

`_O_(_1_)`. Note, you don't have to insert at the end of the list. If you insert at the front of a (singly-linked) list, they are both `O(1)`.

Stack contains 1,2,3:

    [1]->[2]->[3]

Push 5:

    [5]->[1]->[2]->[3]

Pop:

    [1]->[2]->[3] // returning 5

</div>

</div>

<div class="row my-2">

<div><span>Source: <span>stackoverflow.com https://stackoverflow.com/questions/6537150/time-complexity-of-a-stack-adt-implemented-using-a-linked-list#:~:text=For%20a%20doubly%20linked%20list,operations%20of%20enqueue%20and%20dequeue. "What is complexity of `push` and `pop` for a Stack implemented using a LinkedList? Interview Questions Source To Answer"</span></span>   </div>

</div>

</div>

</div>

</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 9\. Design a Stack that supports retrieving the min element in O(1)

</div>

<div>

### Answer:

<div class="answer">

<div>

<div class="mb-2"><span class="h5">Problem</span></div>

<div>

<div class="AnswerBody">

Design a stack that supports push, pop, top, and retrieving the minimum element in constant time.

*   `push(x)` - Push element x onto stack.
*   `pop()` - Removes the element on top of the stack.
*   `top()` - Get the top element.
*   `getMin()` - Retrieve the **minimum** element in the stack.

</div>

</div>

<div>

<div class="AnswerBody">

Using a linked list store the current minimum value. When you add a new number it looks at the previous min and changes the current min to the current value if the current value is lower. Note, each node stores the `min` value _at or below_ it so we don't need to recalculate `min` on pop.

</div>

</div>

<div style="font-size: 14px;">

<div class="mb-3 mt-2"><span class="h5">Implementation</span></div>

<div>

<nav class="mdc-tab-bar">

<div class="mdc-tab-scroller">

<div class="mdc-tab-scroller__scroll-area mdc-tab-scroller__scroll-area--scroll" style="margin-bottom: 0px;">

<div class="mdc-tab-scroller__scroll-content"><button class="mdc-ripple-upgraded mdc-ripple-upgraded--background-focused mdc-tab mdc-tab--min-width mdc-tab--active" aria-selected="true" tabindex="0">

<div class="mdc-tab__content"><span class="mdc-tab__text-label"><span>Java</span> <span class="shadow-text lang-badge java">Java</span></span></div>

<span class="mdc-tab-indicator mdc-tab-indicator--active"><span aria-hidden="true" class="mdc-tab-indicator__content mdc-tab-indicator__content--underline"></span></span></button><button class="mdc-ripple-upgraded mdc-tab mdc-tab--min-width">

<div class="mdc-tab__content"><span class="mdc-tab__text-label"><span>Python</span> <span class="shadow-text lang-badge py">PY</span></span></div>

<span class="mdc-tab-indicator"><span aria-hidden="true" class="mdc-tab-indicator__content mdc-tab-indicator__content--underline"></span></span></button></div>

</div>

</div>

</nav>

</div>

<div class="mt-2">

<div class="AnswerBody">

    class MinStack {

        private class Node {
            int val;
            int min;
            Node next;

            private Node(int val, int min) {
                this(val, min, null);
            }

            private Node(int val, int min, Node next) {
                this.val = val;
                this.min = min;
                this.next = next;
            }
        }

        private Node head;

        public void push(int x) {
            if(head == null) 
                head = new Node(x, x);
            else 
                head = new Node(x, Math.min(x, head.min), head);
        }

        public void pop() {
            head = head.next;
        }

        public int top() {
            return head.val;
        }

        public int getMin() {
            return head.min;
        }
    }

</div>

</div>

</div>

<div class="row my-2">

<div><span>Source: <span>Stackoverflow.com https://stackoverflow.com/ "Design a Stack that supports retrieving the min element in _`O(1)`_ Interview Questions Source To Answer"</span></span>   </div>

</div>

</div>

</div>

</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 10\. Reverse a String using Stack

</div>

<div>

### Answer:

<div class="answer">

<div>

<div>

<div class="AnswerBody">

The followings are the steps to reversing a String using Stack:

1.  `String` to `char[]`.
2.  Create a `Stack`.
3.  **Push** all characters, one by one.
4.  Then **Pop** all characters, one by one and put into the `char[]`.
5.  Finally, convert to the `String`.

</div>

</div>

<div>

<div class="mb-2 mt-2"><span class="h5">Complexity Analysis</span></div>

<div class="hide-small">

<div class="row no-gutters my-2 align-items-end">

<div class="col font-weight-bold text-muted">Time:</div>

<div class="col disable text-center">

<div class="text-muted font-weight-bold justify-content-center">Constant</div>

<div class="complexity amazing first p-1 justify-content-center shadow-text">O(1)</div>

</div>

<div class="col disable text-center">

<div class="text-muted font-weight-bold justify-content-center">Dbl. Logarithmic</div>

<div class="complexity good p-1 justify-content-center shadow-text">O(log log n)</div>

</div>

<div class="col disable text-center">

<div class="text-muted font-weight-bold justify-content-center">Logarithmic</div>

<div class="complexity good p-1 justify-content-center shadow-text">O(log n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold  text-muted justify-content-center">Square Root</div>

<div class="complexity fair p-1 justify-content-center shadow-text ">O(√n)</div>

</div>

<div class="col text-center">

<div class="font-weight-bold  text-muted justify-content-center">Linear</div>

<div class="complexity fair p-1 justify-content-center shadow-text selected-complexity effect7">O(n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold text-muted justify-content-center">Linearithmic</div>

<div class="complexity bad p-1 justify-content-center shadow-text ">O(n log n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold  text-muted justify-content-center">Quadratic</div>

<div class="complexity terrible p-1 justify-content-center shadow-text ">_O_(_n_<sup>2</sup>)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold   text-muted justify-content-center">Exponential</div>

<div class="complexity terrible p-1 justify-content-center shadow-text ">_O_(_2_<sup>n</sup>)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold text-muted">Factorial</div>

<div class="complexity terrible last p-1 justify-content-center shadow-text ">O(n!)</div>

</div>

</div>

</div>

<div class="hide-small">

<div class="row no-gutters my-2 align-items-end">

<div class="col font-weight-bold text-muted">Space:</div>

<div class="col disable text-center">

<div class="text-muted font-weight-bold justify-content-center">Constant</div>

<div class="complexity amazing first p-1 justify-content-center shadow-text">O(1)</div>

</div>

<div class="col disable text-center">

<div class="text-muted font-weight-bold justify-content-center">Dbl. Logarithmic</div>

<div class="complexity good p-1 justify-content-center shadow-text">O(log log n)</div>

</div>

<div class="col disable text-center">

<div class="text-muted font-weight-bold justify-content-center">Logarithmic</div>

<div class="complexity good p-1 justify-content-center shadow-text">O(log n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold  text-muted justify-content-center">Square Root</div>

<div class="complexity fair p-1 justify-content-center shadow-text ">O(√n)</div>

</div>

<div class="col text-center">

<div class="font-weight-bold  text-muted justify-content-center">Linear</div>

<div class="complexity fair p-1 justify-content-center shadow-text selected-complexity effect7">O(n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold text-muted justify-content-center">Linearithmic</div>

<div class="complexity bad p-1 justify-content-center shadow-text ">O(n log n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold   text-muted justify-content-center">Quadratic</div>

<div class="complexity terrible p-1 justify-content-center shadow-text ">_O_(_n_<sup>2</sup>)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold   text-muted justify-content-center">Exponential</div>

<div class="complexity terrible p-1 justify-content-center shadow-text ">_O_(_2_<sup>n</sup>)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold text-muted">Factorial</div>

<div class="complexity terrible last p-1 justify-content-center shadow-text ">O(n!)</div>

</div>

</div>

</div>

<div class="hide-large">

**Time:** <mark>O(n)</mark>

**Space:** <mark>O(n)</mark>

</div>

</div>

<div style="font-size: 14px;">

<div class="mb-3 mt-2"><span class="h5">Implementation</span></div>

<div>

<nav class="mdc-tab-bar">

<div class="mdc-tab-scroller">

<div class="mdc-tab-scroller__scroll-area mdc-tab-scroller__scroll-area--scroll" style="margin-bottom: 0px;">

<div class="mdc-tab-scroller__scroll-content"><button class="mdc-ripple-upgraded mdc-ripple-upgraded--background-focused mdc-tab mdc-tab--min-width mdc-tab--active" aria-selected="true" tabindex="0">

<div class="mdc-tab__content"><span class="mdc-tab__text-label"><span>Java</span> <span class="shadow-text lang-badge java">Java</span></span></div>

<span class="mdc-tab-indicator mdc-tab-indicator--active"><span aria-hidden="true" class="mdc-tab-indicator__content mdc-tab-indicator__content--underline"></span></span></button></div>

</div>

</div>

</nav>

</div>

<div class="mt-2">

<div class="AnswerBody">

    public static String reverse(String str) {
        char[] charArr = str.toCharArray();
        int size = charArr.length;
        Stack stack = new Stack(size);

        int i;
        for (i = 0; i < size; ++i) {
            stack.push(charArr[i]);
        }

        for (i = 0; i < size; ++i) {
            charArr[i] = stack.pop();
        }

        return String.valueOf(charArr);
    }

</div>

</div>

</div>

<div class="row my-2">

<div><span>Source: <span>Stackoverflow.com https://stackoverflow.com/ "Reverse a String using Stack Interview Questions Source To Answer"</span></span>   </div>

</div>

</div>

</div>

</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 11\. Compare Array based vs Linked List stack implementations

</div>

<div>👉🏼 Check all 25 answers https://devinterview.io/data/stacks-interview-questions</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 12\. Explain what are Infix, Prefix and Postfix Expressions?

</div>

<div>👉🏼 Check all 25 answers https://devinterview.io/data/stacks-interview-questions</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 13\. Implement Double Linked List from Stack with min complexity

</div>

<div>👉🏼 Check all 25 answers https://devinterview.io/data/stacks-interview-questions</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 14\. Sort a Stack using another Stack

</div>

<div>👉🏼 Check all 25 answers https://devinterview.io/data/stacks-interview-questions</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 15\. Check if parentheses are balanced using Stack

</div>

<div>👉🏼 Check all 25 answers https://devinterview.io/data/stacks-interview-questions</div>

</div>

Thanks 🙌 for reading and good luck on your next tech interview!  
Explore 3800+ dev interview question here 👉 [Devinterview.io https://devinterview.io/)</div>

</div>
