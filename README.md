# woolfs
class Woolf:
    def __init__(self, name, age, color):
        self.name = name
        self.age = age
        self.color = color
        self.is_sleeping = False

    def sleep(self):
        self.is_sleeping = True
        print(f"{self.name} is now sleeping.")

    def wake_up(self):
        self.is_sleeping = False
        print(f"{self.name} woke up!")

    def description(self):
        return f"{self.name} is a {self.age} years old woolf with {self.color} fur."

def main():
    # Creating a woolf instance
    my_woolf = Woolf("Fluffy", 3, "white")

    # Displaying woolf information
    print(my_woolf.description())

    # Simulating woolf sleeping
    my_woolf.sleep()

    # Simulating woolf waking up
    my_woolf.wake_up()

if __name__ == "__main__":
    main()
