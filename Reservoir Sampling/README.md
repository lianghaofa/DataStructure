Reservoir Sampling
![reservoir](https://user-images.githubusercontent.com/24481784/163451185-ce032bda-a284-49d3-b673-d05e86a2907b.jpg)

    // suppose k is 10

    // the size of bag is 10

    // 1. i <= 10 , put it in the bag

    // 2.i > 10,

    // 2.1 probability 10 / i ,put it in the bag.  if i <= 10, put it in the bag. otherwise throws it away.

    // 2.2 the bag is full, if i <= 10, we should get one out of the bag.  1 / 10
    
    why this works ?
    
    the prosibility of 3 still alive.
    1. when i <= 10, 3 is 100 % alive.
    
    2. 
    2.1 if i == 11, the prosibility of put 11 in the bag is 10 / 11. 
        the prosibility of get 3 out of the bag if 1 / 10 (the size of bag is 10, 1,2,3,4,5,6,7,8,9,10 are in the bag.)
        so the prosibility of 3 still alive is  1 - (10 / 11 * 1 / 10) = 10 / 11
        1 * 10 / 11
    2.2 presumption 3 is still alive
    if i == 12, the prosibility of put 12 in the bag is 11 / 12. 
       the prosibility of get 3 out of the bag if 1 / 10.
       so the prosibility of 3 alive is 1 - (10 / 12 * 1 / 10) = 11 / 12
       1 * 10 / 11 * 11 / 12 
       
    3. when i = n
       
       1 * 10 / 11 * 11 / 12 * ... n-1 / n = 10 / n
    in this case , we take i which less or equal than k for axample.
    
    let's take a > 10 for example.
    
    a = 11.
    
    when i == 11
    10/11, 11 is alive.
    when i == 12
    11/12, 11 is alive.
    10/11 * 11 /12 ... n-1 / n = 10 / n
    
    10/ a + a/a + 1 ... n -1/ n = 10 / n
    
    
    in conclsion, the probability of every element stays in the bag when the game is ending is same.  
       
