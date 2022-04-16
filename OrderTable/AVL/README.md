AVL, a binary tree but keeping balance
how to keep balance ?
Balance Factor ?
Balance Factor = Math.abs ( Height(leftchildren) - Height(rightdren) )
Balance Factor <= 1,  this node is balanced now.
... we process it from down to the top.


4 kind Balance Factor problems:

1.LL problem  Height(leftchildren) - Height(rightdren) = 2
![bb7ba2cd0fff12a8a13e0c16c5180b8](https://user-images.githubusercontent.com/24481784/163669644-992d1323-9f85-42b0-83f5-bf566db59438.png)

how to deal with this?
R rotation.



2.LR problem
![ba9ae895d285cfe14c2916a8db3efa3](https://user-images.githubusercontent.com/24481784/163669651-e1c195a9-9359-4d11-8353-932f53386333.png)

L rotation.

and then R rotation.


3.RR problem  Height(rightdren) - Height(leftchildren) = 2
how to deal with this?
L rotation.

4.RL problem

R rotation.

and then L rotation.

when we delete n node.
LL LR problem
![20645f2098c8d07e9a147192d3c26a4](https://user-images.githubusercontent.com/24481784/163670037-49d44f30-72b0-4ada-b5a8-545df8fcca9c.png)

we must treat this like a LL problem;
![d1a90f4f3c89f337cb83c2d8a963ae9](https://user-images.githubusercontent.com/24481784/163670169-c7e9860c-1009-469f-a37a-fb7511ddc38a.png)


in this case. LL LR both right.
![cac2f7ca02094571be9003abf9a9087](https://user-images.githubusercontent.com/24481784/163670439-6629cbc2-7a3c-44e7-89ba-e7b807c5bcb6.png)
![c5dbcba30e4bb802228f87063060157](https://user-images.githubusercontent.com/24481784/163670445-dbe8ba7a-1ae4-4c2b-80e5-fdf1539c84c1.png)

but s is 4, LR will be wrong.
![ecebdb37afe9a581dd4fdf0ec03236c](https://user-images.githubusercontent.com/24481784/163670531-7b98e48b-4473-441c-b880-0d492ce2b778.png)


treat this like a LR problem may be wrong!



RR RL  problem
we treat this like a RR problem;

LL RR can't happen at the same time.


