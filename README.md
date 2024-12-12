print ("Hello World")

class addition():
    def __init__ (self, a = 0, b = 0):
        self.a = a
        self.b = b
class Add(addition):
    def __init__(self, a= 0, b = 0):
        addition.__init__(self, a, b)

    def forward(self):
        return (self.a + self.b)

add = Add(a = 2, b =3)
print(add.forward())
