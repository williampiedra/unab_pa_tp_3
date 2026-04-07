# unab_pa_tp_3

Objetivos a cumplir por los estudiantes:
● 1. Entender y comprender ejercicios prácticos
● 2. Trabajar en grupos
● 3. Manejo de IDE (cualquiera a elección)
● 4. Manejo de programación básica en Python 3
● 5. Manejo de conceptos vinculados a POO
● 6. Manejo básico de Git y GitHub (crear repositorio y subir archivos)

class Punto:

    def __init__(self, x, y):
        self.x = x
        self.y = y

    def eje_x(self):
        return self.x

    def eje_y(self):
        return self.y

    def impresion(self):
        print(self.x, self.y)

    def opuesto(self):
        x_op = -self.x
        y_op = -self.y
        return Punto(x_op, y_op)

p1 = Punto(2, 5)
print("Eje X:", p1.eje_x())
print("Eje Y:", p1.eje_y())
print("Punto original:")
p1.impresion()
p2 = p1.opuesto()
print("Punto opuesto:")
p2.impresion()


