# Fair-Property-Division

**Problem Statement – **

A father has passed away and in his will has left a number of properties to his multiple children. The only direction in the will is to divide the property as evenly as possible”.
As the executor of the will, you have been given the value of each property. You are to decide how to divide up the property to the children to minimize the difference as much as possible.

**Approach –** 

Solution using recursive method:- 
• The recursive approach is to generate all possible sums from all the values of the properties and to check which solution is the most optimal one. 
• If there are ‘n’ children, that many subsets have to be created and checked.
• So, we end up finding the minimum difference out of all the possible property divisions.


**Algorithm –** 

1)Start 
2)Take the inputs for no child, no of properties 
3)Then input for each property. 
4)If the no or properties is less than equal to no of child 
  a.Then give one property to one child 
  b.If any child is left than assign them 0 value. 
5)Calculate sum of property array 
6)Calculate average of property array based on child left to assign property. 
7)If any property value is greater than current child then directly assign that value to current child. 
8)Otherwise calculate the nearest property value to average which can be assigned to current child. That involve following steps –
  a.Call recursively until value of sum does not become zero and return 1.
  b.Or if the array size becomes zero in that case return 0. 
  c.If above conditions do not match then we check if the property value is greater than sum or not. 
  d.If it is greater than we leave that value and check for further values.
  e.Next we subtract the current array value from sum 
  f.Call recursively this function. 
9)Then we subtract left child by 1. 
10)Subtract property value by the holdings of current child. 
11)Go to step 6 
12)Finish
