# snake-gun-and-water-game-complete-code-in-python
mport random

chance=10
chancesleft=0
yourpoint=0
computerpoint=0


swg=["snake","water","gun"]

while(chancesleft<chance):
    m=input("Enter your choice snace water and gun")
    p = random.choice(swg)
    if(m==p):
        print("Both same no one gets point")
    elif m=="snake" and p=="gun":
        print("You lost")
        computerpoint=computerpoint+1
        chancesleft=chancesleft+1
        print(f"Your point {yourpoint} and computer point is {computerpoint}")
        print(f"You have {chancesleft} chance among {chance} chances")
        print(f"computer choice was {p}")
    elif m=="snake" and p=="water":
        print("You won")
        yourpoint=yourpoint+1
        chancesleft=chancesleft+1
        print(f"Your point {yourpoint} and computer point is {computerpoint}")
        print(f"You have {chancesleft} chance among {chance} chances")
        print(f"computer choice was {p}")
    elif m=="water" and p== "snake":
        print("You lost")
        computerpoint = computerpoint + 1
        chancesleft = chancesleft + 1
        print(f"Your point {yourpoint} and computer point is {computerpoint}")
        print(f"You have {chancesleft} chance among {chance} chances")
        print(f"computer choice was {p}")
    elif m=="water" and p=="gun":
        print("You won")
        yourpoint = yourpoint + 1
        chancesleft = chancesleft + 1
        print(f"Your point {yourpoint} and computer point is {computerpoint}")
        print(f"You have {chancesleft} chance among {chance} chances")
        print(f"computer choice was {p}")
    elif m=="gun" and p=="water":
        print("You lost")
        computerpoint = computerpoint + 1
        chancesleft = chancesleft + 1
        print(f"Your point {yourpoint} and computer point is {computerpoint}")
        print(f"You have {chancesleft} chance among {chance} chances")
        print(f"computer choice was {p}")
    elif m=="gun" and p=="snake":
        print("You won")
        yourpoint = yourpoint + 1
        chancesleft = chancesleft + 1
        print(f"Your point {yourpoint} and computer point is {computerpoint}")
        print(f"You have {chancesleft} chance among {chance} chances")
        print(f"computer choice was {p}")
    else:
        print("Wrong input")
print("game over")
