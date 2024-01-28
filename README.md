# guessing-game

class Guesser:
    def __init__(self, number, lives):
        self.number = number
        self.lives = lives
  
    def guess(self,n):
        if self.lives>0:
            if n != self.number:
                self.lives-=1    
                return False
            else:
                return True
        else:
            raise Exception("Expect error: Omae wa mo shindeiru")
        
a = Guesser(10,3)
print(a.guess(5))
print(a.guess(9))
#print(a.guess(3))
#print(a.guess(10))







