# Circular Queue using Array pointer (not deque)

````py


class Queue:
	# To initialize the object.
	def __init__(self, c):
		self.queue = []  # array
		self.front = self.rear = 0  
		self.capacity = c #must
        	self.size = 0
 
	def queueEnqueue(self, data):
		if(self.capacity == self.size):
			print("\nQueue is full")
		else:
			self.queue.append(data)
		if self.Front is None:
			self.Front = self.Rear = 0	
		else:
			self.Rear = self.Size # where size will increase	
		self.size += 1

	def queueDequeue(self):
		 if self.size <= 0:
			print("udnerflow")
			return 0 #
		else:
			self.queue.pop(0)
			self.size -= 1
			if self.size == 0:
				self.Front = self.Rear = None
			else:
				self.Rear = self.size

	# Function to print queue elements
	def queueDisplay(self)
		if(self.front == self.rear):
			print("\nQueue is Empty")
		# Traverse front to rear to
		# print elements
		for i in self.queue:
			print(i, "<--", end='')

	def queueRear(self):
		if self.Rear is None:
			print("queue is empty")
			raise IndexError
		return self.queue[self.Rear]
	
	def queueFront(self):
		if(self.front == self.rear or self.Rear is None:
			print("\nQueue is Empty")
			raise IndexError
		print(self.queue[self.front])

	def size(self):
		return self.size

# Driver code
if __name__ == '__main__':

	# Create a new queue of
	# capacity 4
	q = Queue(4)

	# Print queue elements
	q.queueDisplay()

	# Inserting elements in the queue
	q.queueEnqueue(20)
	q.queueEnqueue(30)
	q.queueEnqueue(40)
	q.queueEnqueue(50)

	 

# This code is contributed by Amit Mangal



````
