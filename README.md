# Priority Inbox System Design

## Objective

Display the top 10 notifications based on priority and recency.

## Priority Rules

Placement notifications have highest priority.

Result notifications have medium priority.

Event notifications have lowest priority.

Weights:

* Placement = 3
* Result = 2
* Event = 1

## Algorithm

1. Fetch notifications.
2. Assign scores using notification type and timestamp.
3. Sort notifications in descending order.
4. Display top 10 notifications.

## Time Complexity

O(n log n)

## Scalability

For large-scale systems, a Min Heap of size 10 can be used.

Advantages:

* O(log 10) insertion
* Constant memory usage
* Efficient retrieval of top notifications.
