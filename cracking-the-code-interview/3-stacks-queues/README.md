# Statcks and Queues

## Implementing as Stack

    class Stack {
        Node top;
        Node pop() {
            if (top != null) {
                Object item = top.data;
                top = top.next;
                return item;
            }
            return null;
        }
        void push(Object item) {
            Node t = new Node(item);
            t.next = top;
            top = t;
        }
    }

## Implementing a Queue

    class Queue {
        Node first, last;
        void enqueue(Object item) {
            if (!first) {
                back = new Node(item);
                first = back;
            } else {
                back.next = new Node(item);
                back = back.next;
            }
        }
        Node deque(Node n) {
            if (front != null) {
                Object item = front.data;
                front = front.next;
                return item;
            }
            return null;
        }

    }

## Exercises
|No.|Title|Solution|
|---|-----|--------|
|3.1|[Use a single array to implement three stacks](three-stacks)|[Java1](three-stacks/ThreeStacks1.java) [Java2](three-stacks/ThreeStacks2.java)|
|3.2|[Stack with push, pop, min in O(1) time](stack-min)][Java1](stack-min/StackMin1.java) [Java2](stack-min/StackMin2.java)|
|3.3|[Set of stacks, create a new stack once previous capacity](set-of-stacks)|[Java](set-of-stacks/SetOfStacks.java)|
|3.4|[Hanoi with stacks](hanoi-with-stacks)|[Java](hanoi-with-stacks/HanoiWithStacks.java)|
|3.5|[Implenting a queue using two stacks](queue-two-stacks)|[Java](queue-two-stacks/MyQueue.java)|
|3.6|[Sort a stack using push, pop, peak, isEmpty](sort-stack)|[Java](sort-stack/SortStack.java)|
