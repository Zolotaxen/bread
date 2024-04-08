# bread
class Bread:
    def __init__(self, type_of_bread, weight_g):
        self.type_of_bread = type_of_bread
        self.weight_g = weight_g
        self.is_toasted = False  # Initially bread is not toasted

    def toast(self):
        self.is_toasted = True
        print(f"{self.type_of_bread} bread is now toasted!")

    def describe(self):
        toasted_status = "toasted" if self.is_toasted else "not toasted"
        print(f"This is {self.type_of_bread} bread weighing {self.weight_g}g, {toasted_status}.")

# Example usage:
if __name__ == "__main__":
    # Create an instance of Bread
    my_bread = Bread("Whole Wheat", 300)

    # Describe the bread
    my_bread.describe()

    # Toast the bread
    my_bread.toast()

    # Describe the bread again
    my_bread.describe()
