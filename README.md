# rockpaper
#test
import random as rm

l=["rock","paper","scissor"]
ccount=0
ucount=0
i=1
while (i<=5):
        i=i+1
        a=int(input('''
                    1 for rock
                    2 for paper
                    3 for scissor
                    
                    
                    '''))
        
        if(a==1):
            uchoice="rock"
        elif(a==2):
            uchoice="paper"
        elif(a==3):
            uchoice="scissor"
    
        cchoice=rm.choice(l)
        if(cchoice==uchoice):
            print("draw")
            print("computer chose",cchoice,"\n","user choose",uchoice)
            ucount+=1
            ccount+=1
        elif(cchoice=="rock"and uchoice=="paper"):
            print("user +1 score addition")
            print("computer chose",cchoice,"\n","user choose",uchoice)
            ucount=ucount+1
        elif(cchoice=="paper"and uchoice=="scissor"):
            print("user +1 score addition")
            print("computer chose",cchoice,"\n","user choose",uchoice)
            ucount=ucount+1
        elif(cchoice=="scissor"and uchoice=="rock"):
            print("user +1 score addition")
            print("computer chose",cchoice,"\n","user choose",uchoice)
            ucount=ucount+1
        elif(uchoice=="rock"and cchoice=="paper"):
            print("computer +1 score addition")
            print("computer chose",cchoice,"\n","user choose",uchoice)
            ccount=ccount+1
        elif(uchoice=="paper"and cchoice=="scissor"):
            print("computer +1 score addition")
            print("computer chose",cchoice,"\n","user choose",uchoice)
            ccount=ccount+1
        elif(uchoice=="scissor" and cchoice=="rock"):
            print("computer+1 score addition")
            print("computer chose",cchoice,"\n","user choose",uchoice)
            ccount=ccount+1

print("\n Final leaderboard")
if(ucount==ccount):
    print("game is draw")
    print("computer score",ccount,"usercount",ucount)
elif(ucount>ccount):
    print("user win the game")
    print("computer score",ccount,"usercount",ucount)
elif(ucount<ccount):
    print("computer win the game")
    print("computer score",ccount,"usercount",ucount)
        


    



    
