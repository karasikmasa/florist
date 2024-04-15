# florist
class Flower:
    def __init__(self, name, color, price):
        self.name = name
        self.color = color
        self.price = price

class Florist:
    def __init__(self):
        self.inventory = []

    def add_flower(self, flower):
        self.inventory.append(flower)

    def display_inventory(self):
        print("Florist Inventory:")
        for flower in self.inventory:
            print(f"Name: {flower.name}, Color: {flower.color}, Price: ${flower.price}")

def main():
    florist = Florist()

    # Adding some flowers to the inventory
    rose = Flower("Rose", "Red", 10)
    tulip = Flower("Tulip", "Yellow", 8)
    lily = Flower("Lily", "White", 12)

    florist.add_flower(rose)
    florist.add_flower(tulip)
    florist.add_flower(lily)

    # Displaying the inventory
    florist.display_inventory()

if __name__ == "__main__":
    main()
