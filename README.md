# 1class DoorHandle:
    def __init__(self):
        self.is_locked = False
        self.is_open = False
    
    def lock(self):
        if not self.is_open:
            self.is_locked = True
            print("The door is now locked.")
        else:
            print("Cannot lock the door while it's open.")
    
    def unlock(self):
        if not self.is_open:
            self.is_locked = False
            print("The door is now unlocked.")
        else:
            print("Cannot unlock the door while it's open.")
    
    def open(self):
        if not self.is_locked:
            self.is_open = True
            print("The door is now open.")
        else:
            print("The door is locked. Unlock it first.")
    
    def close(self):
        self.is_open = False
        print("The door is now closed.")

# Example usage
handle = DoorHandle()
handle.lock()
handle.unlock()
handle.open()
handle.close()
