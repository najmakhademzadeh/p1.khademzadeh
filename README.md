# p1.khademzadeh
from multiprocessing import Process
def test2(x):
for i in range(6):
print(x)
if __name__ == '__main__':
p1 = Process(target=test2, args=("p1",))
p2 = Process(target=test2, args=("p2",))
p1.start()
p2.start()
p2.join() p1.join()
