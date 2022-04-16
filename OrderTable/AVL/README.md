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
