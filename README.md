class Tvarina:
    def __init__(self, name, age):
        self.name = name
        self.age = age
    
    def make_sound(self):
        pass
    
    def info(self):
        return f"Я {self.name}, мені {self.age} років."

class Sobaka(Tvarina):
    def __init__(self, name, age, breed):
        super().__init__(name, age)
        self.breed = breed
    
    def make_sound(self):
        return "Гав-гав!"
    
    def info(self):
        return f"Я собака {self.name}, породи {self.breed}, мені {self.age} років."

class Kit(Tvarina):
    def __init__(self, name, age, color):
        super().__init__(name, age)
        self.color = color
    
    def make_sound(self):
        return "Мяу-мяу!"
    
    def info(self):
        return f"Я кіт {self.name}, маю {self.color} колір, мені {self.age} років."

sobaka = Sobaka("Рекс", 3, "Лабрадор")
kit = Kit("Мурзик", 2, "сірий")

print(sobaka.info())
print(sobaka.make_sound())
print(kit.info())
print(kit.make_sound())
