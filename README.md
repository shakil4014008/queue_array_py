# queue_array_py

````
class Queue:
    def __init__(self, c):
        self.queue = [] #array
        self.front = self.rear = 0 # 2 variables to track front and rear
        self.capacity = c
        self.size  = 0

    def enqueue(self, data):
        if self.capacity == self.size:
            print("\n Queue is full")
        else:
            self.queue.append(data)
            self.rear += 1
            self.size += 1

    def dequeue(self):
        if self.size == 0:
            print("\nQueue is empty")
        else:
            x = self.queue.pop(0)
            self.rear -= 1
            self.size -= 1
    def print_queue(self):
        if self.size == 0:
            print("Queue is empty")
        for item in self.queue:
            print(item, "<--", end='')


q  = Queue(4)
q.enqueue(2)
q.enqueue(4)
q.enqueue(6)
q.enqueue(8)
q.dequeue()
q.dequeue()
q.print_queue()


````
