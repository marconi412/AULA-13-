#criar classe 
class animal(): 
#construcao de classe
    def __init__(self, name, weight, color):
#atributos
        self.nome = name
        self.peso = weight
        self.cordopelo = color

    def imprimirdados(self):
        return("nome: %s \npeso: %s" %(self.nome, self.peso))
    
    def latir(self, barulho):
        print(barulho)

        #instanciando objeto cachorro
caozinho = animal("marlene", 7.9, "caramelo")
gato = animal("cibele", 4.5, "cinza")

#metodo do objeto criado 
print(caozinho.imprimirdados())
caozinho.latir("au au")

print(gato.imprimirdados())
gato.latir("miau")

class livro():
    def __init__(self, titulo, isbn):
        self.titulo = "o monge e o executivo"
        self.isbn = 9988888
        print("construtor chamado para criar objeto de classe")
        
    def imprime(self):
        print("foi criado o livro %s e isbn %d" %( self.titulo, self.isbn))

livro1 = livro("o monge e o executivo", 9988888)

print (livro1.imprime())

class Pessoa ():
    def __init__ (self, name, age):
        self.nome = name
        self.idade= age
        
    def nascimento(self, idade):
        return (2024 - idade)

        pessoa1 = Pessoa ("maria", 35)
pessoa1.nome
pessoa1.idade
pessoa1.nascimento(35)

listadepessoas = []
for i in range (5):
    nome = str (input("nome:"))
    idade = int (input("idade:"))
    pessoa = Pessoa(nome, idade)
    listadepessoas.append(pessoa)

for objeto in range(len(listadepessoas)):
    print("nome: %s, idade: %d " %(listadepessoas[objeto].nome, listadepessoas[objeto].idade))
        
