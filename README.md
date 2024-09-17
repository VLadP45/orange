# orangeclass Orange:
    def __init__(self, size):
        self.size = size  # Size of the orange (in some unit)
        self.peeled = False
        self.eaten = False

    def peel(self):
        if not self.peeled:
            self.peeled = True
            print("You have peeled the orange!")
        else:
            print("The orange is already peeled.")

    def eat(self):
        if self.peeled and not self.eaten:
            self.eaten = True
            print("You eat the orange. Yum!")
        elif not self.peeled:
            print("You need to peel the orange first.")
        else:
            print("The orange has already been eaten.")

# Example of using the Orange class
my_orange = Orange(size=5)
my_orange.peel()  # Peels the orange
my_orange.eat()   # Eats the orange
