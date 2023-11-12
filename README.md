# lab-task-5-shakeel-ahmad
implement  a basic queue using in arraybin python include method of enqueu,dequeue checking it if the queue is empty and fiding the size of the queue 


class Queue:
    def _init_(self):
        self.items = []

    def is_empty(self):
        return len(self.items) == 0

    def enqueue(self, item):
        self.items.append(item)

    def dequeue(self):
        if not self.is_empty():
            return self.items.pop(0)
        else:
            print("Queue is empty. Cannot dequeue.")

    def size(self):
        return len(self.items)

# Example Usage:
my_queue = Queue()

print("Is the queue empty?", my_queue.is_empty())  # Output: True

my_queue.enqueue(1)
my_queue.enqueue(2)
my_queue.enqueue(3)

print("Queue size:", my_queue.size())  # Output: 3

print("Dequeue:", my_queue.dequeue())  # Output: 1

print("Is the queue empty?", my_queue.is_empty())  # Output: False

print("Queue size:", my_queue.size())  # Output: 2
