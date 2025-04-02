import random
import sys
print("""~~~~~~~~~~cricket~~~~~~~~~~ 

Here is a game of cricket using numbers
Instructions:
1.First,you have to choose heads or tails.
2.If you win the toss then you can choose batting or bowling while computer will be your opponent.
3.After choosing,the innings will start and The innings will end after either the three wickets fell or the overs end.
4.you have to choose a number randomly from 1 to 6
5.The computer will also choose a number randomly.
6.While bowling, if the number selected by you  and computer is different, then the computer's number will add to its runs.
  If the number selected by you and computer is same, then the computer will lose its wicket.
7.While batting, if the number selected by you and computer is different, then your number will add to your runs.
  If the number selected by you and computer is same, then you will lose your wicket.
8.Each player will get 2 overs and 2 overs 2 wickets for batting and bowling.
9.the person with maximum score wins..
""")
print("welcome to Cricket")
num=(int(input("choose number of overs from a range of 1-5 : ")))
wickets=num
balls=num*6
mlist=[1,2]
nlist=[1,2]
systemopt=[1,2]
sopt=random.choice(systemopt)
random_tossing=random.choice(mlist)
random_borbow=random.choice(nlist)
mine=0
cine=0
my_cho=(input("choose heads or tails:")).lower()
if(my_cho!="heads" and my_cho!="tails"):
    print("invalid selection")
    sys.exit()
if(random_tossing==1 and my_cho=="heads"):
    print("\nyou won the toss")
    choice=(input("batting or bowling :")).lower()
    mine=choice
    if(choice!="batting" and choice!="bowling"):
        print("invalid choice")
        sys.exit()
    
elif(random_tossing==2 and my_cho=="tails"):
    print("\nyou won the toss")
    choice=(input("batting or bowling:")).lower()
    mine=choice
    if(choice!="batting" and choice!="bowling"):
        print("invalid choice")
        sys.exit()
else:
    print("\nyou lost the toss ")
    if(sopt==1):
        print("computer choose batting")
        cine="batting"
    else:
        print("computer choose bowling")
        cine="bowling"
#---------- First Innings Begins ----------#
listofr=[1,2,3,4,5,6]
myscore_1=0
wickets_f=0
balls_f=0
cscore_1=0
while wickets_f!=wickets and balls_f!=balls:
    if(balls_f==6):
        print("----------End of First over--------")
        print("----------second over starts--------")
    mychoicees=(input("choose a number from 1 to 6 :"))
    mychoicee=int(mychoicees)
    cchoice=random.choice(listofr)
    if(mychoicee<1 or mychoicee >6):
        print("choose only between 1 to 6")
        balls_f-=1
    else:
        print("your choice =",mychoicee)
        print("computer choice =",cchoice)
        if(mychoicee==cchoice):
            print("-----wicket out----")
            if(mine=="batting" or cine=="bowling"):
                wickets_f+=1
                cscore_1+=cchoice
            elif(mine=="bowling" or cine=="batting"):
                wickets_f+=1
                myscore_1+=mychoicee
        else:
            if(mine=="batting" or cine=="bowling"):
                myscore_1+=mychoicee
            elif(mine=="bowling" or cine=="batting"):
                cscore_1+=cchoice
    balls_f+=1
    if(mine=="batting"):
        print("your score:",myscore_1)
    elif(cine=="batting"):
        print("Computer's Score :",cscore_1)
print("end of the first innings")
print("....Start of second innings...")
#---------- Second Innings Begins ----------#
mine,cine=cine,mine
print("Now you are ",mine)
myscore_2=0
wickets_s=0
balls_s=0
cscore_2=0
while wickets_s!=wickets and balls_s!=balls:
    if(balls_s==6):
        print("----------End of First over--------")
        print("----------second over starts--------")
    mychoicees=(input("choose a number from 1 to 6 :"))
    mychoice=int(mychoicees)
    cchoice=random.choice(listofr)
    if(mychoice<1 or mychoice >6):
        print("choose only between 1 to 6")
    else:
        print("your choice =",mychoice)
        print("computer choice =",cchoice)
        if(mychoice==cchoice):
            print("----wicket out----")
            if(mine=="batting" or cine=="bowling"):
                wickets_s+=1
                cscore_2+=cchoice
                
            elif(mine=="bowling" or cine=="batting"):
                wickets_s+=1
                myscore_2+=mychoice
                
        else:
            if(mine=="batting" or cine=="bowling"):
                myscore_2+=mychoice
            elif(mine=="bowling" or cine=="batting"):
                cscore_2+=cchoice
    balls_s+=1
    if(mine=="batting"):
        print("your score:",myscore_2)
    elif(cine=="batting"):
        print("Computer's Score :",cscore_2)
print("End of second innings")
myfinal=myscore_1+myscore_2
comfinal=cscore_1+cscore_2
print("your Final Score:",myfinal,"/","Computer's Final Score",comfinal)
if(myfinal>comfinal):
    print("Congratulations u won the match")
elif(myfinal==comfinal):
    print("Noone wins..!It's a tie")
else:
    print("computer won the match..!Better luck next time")
