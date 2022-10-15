from pydoc import describe
import random as rand
import time


def beginF():
    areYouReady = str(input("Are you ready ???\n"))
    global secretNumber
    if areYouReady.lower() == "yes":
        print("I am guessing a number")
        for eachSign in range(8):
            print('.', end=' ', flush=True)
            time.sleep(0.25)
        secretNumber = rand.randint(1, 10)
        print('\nSSSHHH:\n-----------------------------\n %s \n------------------------------\n' % (secretNumber))
        print("I am all set! :)")
        startGame()
    elif areYouReady.lower() == "no":
        byeMessage()


def startGame():
    decision = int(input('Make a decision[1-10], brotha: '))
    if secretNumber > decision:
        print("Heyo, my number is greater than Yours ;)")
        startGame()
    elif secretNumber < decision:
        print("My number is less than yours")
        startGame()
    elif secretNumber == decision:
        print('\n***************************\nYOU ARE THE BOSS.\n***************************' )
        print("I was guessing %s !" % (secretNumber))

def byeMessage():
    print('G O O D B Y E ! ! !')


beginF()
