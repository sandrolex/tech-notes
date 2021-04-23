# Big O Examples

## O(1) Constant
    def func_constant(values):
        '''
        Prints first item in a list of values.
        '''
        print values[0]
    
    func_constant([1,2,3])
    1
   

## O(n) Linear
    def func_lin(lst):
        '''
        Takes in list and prints out all values
        '''
        for val in lst:
            print val
        
    func_lin([1,2,3])
    1
    2
    3


## O(n^2) Quadratic
    def func_quad(lst):
        '''
        Prints pairs for every item in list.
        '''
        for item_1 in lst:
            for item_2 in lst:
                print item_1,item_2

    lst = [0, 1, 2, 3]

    func_quad(lst)
    0 0
    0 1
    0 2
    0 3
    1 0
    1 1
    1 2
    1 3
    2 0
    2 1
    2 2
    2 3
    3 0
    3 1
    3 2
    3 3


## Big-O Complexity
![From stack overflow](https://i.stack.imgur.com/WcBRI.png)



* [Notation](https://stackoverflow.com/questions/487258/what-is-a-plain-english-explanation-of-big-o-notation/487278#487278)
* [Examples](https://stackoverflow.com/questions/2307283/what-does-olog-n-mean-exactly)
