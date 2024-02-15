# cod-dv
class Door:
    def __init__(self, code):
        self.code = code
        self.locked = True

    def unlock(self, entered_code):
        if entered_code == self.code:
            self.locked = False
            print("Door unlocked!")
        else:
            print("Incorrect code. Door remains locked.")

# Example usage
if __name__ == "__main__":
    # Define the door code
    door_code = "1234"

    # Create a door object
    door = Door(door_code)

    # Attempt to unlock the door
    entered_code = input("Enter the door code: ")
    door.unlock(entered_code)
