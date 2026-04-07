# unab_pa_tp_3

Objetivos a cumplir por los estudiantes:
● 1. Entender y comprender ejercicios prácticos
● 2. Trabajar en grupos
● 3. Manejo de IDE (cualquiera a elección)
● 4. Manejo de programación básica en Python 3
● 5. Manejo de conceptos vinculados a POO
● 6. Manejo básico de Git y GitHub (crear repositorio y subir archivos)

Ejercicio 2
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

Ejercicio 3
class Linea:
def __init__(self, punto_a, punto_b):
self.punto_a = punto_a
self.punto_b = punto_b
def mueve_derecha(self, d):
self.punto_a.x = self.punto_a.x + d
self.punto_b.x = self.punto_b.x + d

def mueve_izquierda(self, d):
self.punto_a.x = self.punto_a.x - d
self.punto_b.x = self.punto_b.x - d

def mueve_arriba(self, d):
self.punto_a.y = self.punto_a.y + d
self.punto_b.y = self.punto_b.y + d

def mueve_abajo(self, d):
self.punto_a.y = self.punto_a.y - d
self.punto_b.y = self.punto_b.y - d

def impresion(self):
return str(self.punto_a.x) + " " + str(self.punto_a.y) + " - " + str(self.punto_b.x) + " " + str(self.punto_b.y)

Ejercicio 4

class Cancion:
def __init__(self, titulo, autor):
self.titulo = titulo
self.autor = autor
def get_titulo(self):
return self.titulo

def get_autor(self):
return self.autor

def set_titulo(self, titulo):
self.titulo = titulo

def set_autor(self, autor):
self.autor = autor

Ejercicio 5 

class Persona:
def __init__(self, nombre):
self.nombre = nombre

def get_nombre(self):
return self.nombre

def set_nombre(self, nombre):
self.nombre = nombre

class Libro:
def __init__(self, titulo, autor, isbn, paginas, edicion, editorial, ciudad, pais, fecha):
self.titulo = titulo
self.autor = autor
self.isbn = isbn
self.paginas = paginas
self.edicion = edicion
self.editorial = editorial
self.ciudad = ciudad
self.pais = pais
self.fecha = fecha

def get_titulo(self):
return self.titulo

def set_titulo(self, titulo):
self.titulo = titulo

def get_autor(self):
return self.autor

def set_autor(self, autor):
self.autor = autor

def leer(self):
print("Ingrese los datos del libro")
self.titulo = input("Titulo: ")
nombre = input("Autor: ")
self.autor = Persona(nombre)
self.isbn = input("ISBN: ")
self.paginas = input("Paginas: ")
self.edicion = input("Edicion: ")
self.editorial = input("Editorial: ")
self.ciudad = input("Ciudad: ")
self.pais = input("Pais: ")
self.fecha = input("Fecha: ")

def mostrar(self):
print("Titulo:", self.titulo, self.edicion)
print("Autor:", self.autor.get_nombre())
print("ISBN:", self.isbn)
print(self.editorial + ", " + self.ciudad + " (" + self.pais + ")")
print(self.fecha)
print(self.paginas, "paginas")
