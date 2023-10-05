# Dice-Sum-Solution-And-Python-Code

# Problem
Roll a die n times, what is the probability that their sum will be equal to k.

# Solution
First, we need to find the probabilities of sum of rolled dice, which is equal to the number of ways to get the sum equal to k divided by the total number of possibilities, which is equal to 6n.
The minimum sum is equal to 1*n and the maximum sum is equal to 6*n.
If you calculate possible sums of rolled dice for n = 1, 2, 3 and 4, you can notice a pattern. If we roll two dice, the sum of values can be obtained from the sum of values of the case that we roll two dice. In the case of three dice, the sum of values can be obtained from the sum of values of the case that we roll two dice and so on. 
The resulting relationship is shown in the tables below.
 
 ![image](https://github.com/tamarakirakosyan/Dice-Sum-Solution-And-Python-Code/assets/46844022/4b51a7d7-7a8e-43fb-8ce9-e7c73281eb7a)

 ![image](https://github.com/tamarakirakosyan/Dice-Sum-Solution-And-Python-Code/assets/46844022/b6d5a228-1a51-453c-9255-14ba3a8770d3)

 ![image](https://github.com/tamarakirakosyan/Dice-Sum-Solution-And-Python-Code/assets/46844022/e626984c-0455-45ed-8eba-ba7c976a261b)

 ![image](https://github.com/tamarakirakosyan/Dice-Sum-Solution-And-Python-Code/assets/46844022/50ff79b6-83cd-4615-b548-e4e9e4df8fff) 

The function dice_sum_probs in the python code calculates the probabilities of sum of the dice values.
And the function create_dict_of_sums_probs creates a dictionary with the sums of the rolled dice and their probabilities.
