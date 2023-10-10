# day_13_Python
############ DEBUGGING #####################

# # Describe Problem
# Undebugged problem
# Find out solutions to make it print 'You Got It'
# def my_function():
#   for i in range(1, 20):
#     if i == 20:
#       print("You got it")
# my_function()

# 1️⃣ My solution ⬇︎
def my_function():
   for i in range(1, 20):
     if i + 1 > 0 and i + 1 < 21:
       print("You got it")
       return i 
my_function()

# 2️⃣ Alternative solution ⬇︎
def my_function():
   for i in range(1, 20):
     if i + 1 > 0 and i + 1 < 21:
       print("You got it")
       return i 
my_function()

# # Reproduce the Bug
# from random import randint
# dice_imgs = ["❶", "❷", "❸", "❹", "❺", "❻"]
# dice_num = randint(1, 6)
# print(dice_imgs[dice_num])

# randint () includes both limits(upper and lower limits)
from random import randint
# The list dice_imgs stands for 0 - 5, so the printed dice_num should be starting from 0 and ending to 5, instead of (1, 6)
dice_imgs = ["❶", "❷", "❸", "❹", "❺", "❻"]
dice_num = randint(0, 5)
print(dice_imgs[dice_num])











