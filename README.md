# roseclass Rose:
    def __init__(self, petals):
        self.petals = petals  # The number of petals on the rose

    def pick_petal(self):
        if self.petals > 0:
            self.petals -= 1
            print(f"You picked a petal! {self.petals} petals left.")
        else:
            print("No petals left. The rose is bare.")

# Example usage:
my_rose = Rose(petals=7)  # A rose with 7 petals

# Simulating picking all petals
while my_rose.petals > 0:
    my_rose.pick_petal()

my_rose.pick_petal()  # Trying to pick a petal after the rose is bare
