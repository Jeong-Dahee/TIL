# TIL
Today I Learned ๐ค๐ : ์ค๋์ ๊ณต๋ถ

```python
# (๋ฌธ์ . README.md ๋ฐ ํ๋จ ๋งํฌ ์ฐธ์กฐ) ์์คํค์ฝ๋๋ฅผ ์ด์ฉํ ๋ณด๋ฌผ์ฌ ๊ฒ์ ๋ง๋ค๊ธฐ

# ์์คํค์ฝ๋๋ ์ผ๋ฐ์ ์ธ ๋ฌธ์์ด(string)์ฒ๋ผ "" ์ด ์๋, ๋ค์ค๋ธ๋ก๋ฌธ์์ด(multi block string)์ ''' ''' ์ ์ฌ์ฉํด์ผํจ
print('''
*******************************************************************************
          |                   |                  |                     |
 _________|________________.=""_;=.______________|_____________________|_______
|                   |  ,-"_,=""     `"=.|                  |
|___________________|__"=._o`"-._        `"=.______________|___________________
          |                `"=._o`"=._      _`"=._                     |
 _________|_____________________:=._o "=._."_.-="'"=.__________________|_______
|                   |    __.--" , ; `"=._o." ,-"""-._ ".   |
|___________________|_._"  ,. .` ` `` ,  `"-._"-._   ". '__|___________________
          |           |o`"=._` , "` `; .". ,  "-._"-._; ;              |
 _________|___________| ;`-.o`"=._; ." ` '`."\` . "-._ /_______________|_______
|                   | |o;    `"-.o`"=._``  '` " ,__.--o;   |
|___________________|_| ;     (#) `-.o `"=.`_.--"_o.-; ;___|___________________
____/______/______/___|o;._    "      `".o|o_.--"    ;o;____/______/______/____
/______/______/______/_"=._o--._        ; | ;        ; ;/______/______/______/_
____/______/______/______/__"=._o--._   ;o|o;     _._;o;____/______/______/____
/______/______/______/______/____"=._o._; | ;_.--"o.--"_/______/______/______/_
____/______/______/______/______/_____"=.o|o_.--""___/______/______/______/____
/______/______/______/______/______/______/______/______/______/______/_____ /
*******************************************************************************
''')
print("Welcome to Treasure Island.")
print("Your mission is to find the treasure.")

#https://www.draw.io/?lightbox=1&highlight=0000ff&edit=_blank&layers=1&nav=1&title=Treasure%20Island%20Conditional.drawio#Uhttps%3A%2F%2Fdrive.google.com%2Fuc%3Fid%3D1oDe4ehjWZipYRsVfeAx2HyB7LCQ8_Fvi%26export%3Ddownload

#Write your code below this line ๐
#๋ด ์ฝ๋
Q1 = input("do you want to go left or right? ").lower()
if Q1 == "left":
    Q2 = input("will you swim or wait? ").lower()
    if Q2 == "wait":
        Q3 = input("which door do you want to walk in? Red, Yellow or Blue? "
                   ).lower()
        if Q3 == "red":
            print("you are Burned by fire.\n -Game Over-")
        elif Q3 == "yellow":
            print("you win!")
        elif Q3 == "blue":
            print("you are eaten by beasts.\n -Game Over-")
        else:
            print("-Game Over-")
    else:
        print("you attacked by trout.\n -Game Over-")
else:
    print("you fell into a hole.\n -Game Over-")

# ์ ๋ต
print('''
*******************************************************************************
          |                   |                  |                     |
 _________|________________.=""_;=.______________|_____________________|_______
|                   |  ,-"_,=""     `"=.|                  |
|___________________|__"=._o`"-._        `"=.______________|___________________
          |                `"=._o`"=._      _`"=._                     |
 _________|_____________________:=._o "=._."_.-="'"=.__________________|_______
|                   |    __.--" , ; `"=._o." ,-"""-._ ".   |
|___________________|_._"  ,. .` ` `` ,  `"-._"-._   ". '__|___________________
          |           |o`"=._` , "` `; .". ,  "-._"-._; ;              |
 _________|___________| ;`-.o`"=._; ." ` '`."\` . "-._ /_______________|_______
|                   | |o;    `"-.o`"=._``  '` " ,__.--o;   |
|___________________|_| ;     (#) `-.o `"=.`_.--"_o.-; ;___|___________________
____/______/______/___|o;._    "      `".o|o_.--"    ;o;____/______/______/____
/______/______/______/_"=._o--._        ; | ;        ; ;/______/______/______/_
____/______/______/______/__"=._o--._   ;o|o;     _._;o;____/______/______/____
/______/______/______/______/____"=._o._; | ;_.--"o.--"_/______/______/______/_
____/______/______/______/______/_____"=.o|o_.--""___/______/______/______/____
/______/______/______/______/______/______/______/______/______/______/_____ /
*******************************************************************************
''')
print("Welcome to Treasure Island.")
print("Your mission is to find the treasure.")

# ์ด์ค์ผ์ดํ ์ฒ๋ฆฌ : ์ํฌ์คํธ๋กํผ(')๋ฅผ ๋ฌธ์๋ก ์ธ์ํ๊ฒํ๋ ค๋ฉด ๋ฐฑ์ฌ๋์(\)๋ฅผ ์์์จ์ค๋ค 
Q1 = input(
    'You\'re at a cross road. Where do you want to go? Type "left" or "right" \n'
).lower() 
if Q1 == 'left':
    Q2 = input(
        'You\'ve come to a lake. There is an island in the middle of the lake. Type "wait" to wait for a boat. Type "swim" to swim across. \n'
    ).lower()
    if Q2 == 'wait':
        Q3 = input(
            "You arrive at the island unharmed. There is a house with 3 doors. One red, one yellow and one blue. Which colour do you choose? \n"
        )
        if Q3 == 'red':
            print("It's a room full of fire. Game Over.")
        elif choice3 == "yellow":
            print("You found the treasure! You Win!")
        elif choice3 == "blue":
            print("You enter a room of beasts. Game Over.")
        else:
            print("You chose a door that doesn't exist. Game Over.")
    else:
        print("You get attacked by an angry trout. Game Over.")
else:
    print("You fell into a hole. Game Over.")

```
dsdsds
