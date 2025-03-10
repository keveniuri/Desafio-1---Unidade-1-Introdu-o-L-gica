# Calculadora de Formas Geométricas
Este é um programa simples em Python que permite calcular a área e o perímetro de formas geométricas, como retângulos e círculos, com base nos valores fornecidos pelo usuário.
# 🛠️Tecnologias Utilizadas
•	Python 3
•	Programação Orientada a Objetos (POO)
•	Classes e Métodos Abstratos (ABC)
# 🖥️instalação 
Para rodar o programa, certifique-se de que o Python 3 está instalado no seu computador.
1.	Clone este repositório: 
2.	git clone https:(https://github.com/keveniuri/Desafio-1---Unidade-1-Introdu-o-L-gica/blob/main/c%C3%B3digo)
3.	Execute o programa: 
4.	python formas_geometricas.py
# 🚀Como usar 
Ao executar o programa, você será solicitado a escolher uma forma geométrica (retângulo ou círculo) e inserir os valores necessários para os cálculos.
# ⚡Exemplo de uso para um Retângulo:
Digite o tipo de forma (retangulo ou circulo): retangulo
Digite a largura do retângulo: 10
Digite a altura do retângulo: 5
# 📌saída esperada 
Retangulo:
Área: 50.0
Perímetro: 30.0
# ⚡Exemplo de uso para um Círculo:
Digite o tipo de forma (retangulo ou circulo): circulo
Digite o raio do círculo: 7
# 📌saída esperada 
Circulo:
Área: 153.9385
Perímetro: 43.982
# ✉️estrutura do Código 
O programa segue a abordagem de Programação Orientada a Objetos (POO), utilizando conceitos fundamentais como abstração, herança, encapsulamento e polimorfismo. Abaixo, explicamos como cada um deles foi aplicado no código.
# ⚡Abstração
A classe abstrata FormaGeometrica define a estrutura básica para qualquer forma geométrica, sem se preocupar com a implementação dos métodos. Isso permite criar diferentes formas geométricas sem precisar reescrever o código base.
from abc import ABC, abstractmethod

class FormaGeometrica(ABC):
    @abstractmethod
    def calcular_area(self):
        pass
    
    @abstractmethod
    def calcular_perimetro(self):
        pass
# ⚡Herança 
As classes Retangulo e Circulo herdam da classe FormaGeometrica, garantindo que todas as formas geométricas implementem os métodos calcular_area() e calcular_perimetro().
class Retangulo(FormaGeometrica):
    def __init__(self, largura, altura):
        self.largura = largura
        self.altura = altura
    
    def calcular_area(self):
        return self.largura * self.altura
    
    def calcular_perimetro(self):
        return 2 * (self.largura + self.altura)

  # ⚡Encapsulamento
  Os atributos largura, altura e raio são protegidos dentro das classes e só podem ser acessados e modificados através dos métodos definidos.
  # ⚡ Polimorfismo
Como Retangulo e Circulo implementam calcular_area() e calcular_perimetro() de maneiras diferentes, podemos chamar esses métodos sem precisar saber qual é o tipo específico do objeto.
def exibir_informacoes(forma: FormaGeometrica):
    print(f"Área: {forma.calcular_area()}")
    print(f"Perímetro: {forma.calcular_perimetro()}")
Isso permite que o código seja mais flexível e reutilizável.
# 🤝 Contribuição
Contribuições são bem-vindas! Para contribuir:
1.	Faça um fork do repositório.
2.	Crie uma nova branch: git checkout -b minha-feature
3.	Adicione suas alterações: git add .
4.	Faça um commit: git commit -m 'Adicionando nova funcionalidade'
5.	Envie as alterações: git push origin minha-feature
6.	Abra um Pull Request.
# 📝Licença
Este projeto está sob a licença MIT. Sinta-se à vontade para utilizá-lo e modificá-lo.
# Referência usada:

Livros:

Python 3 Object-Oriented Programming Second edition Dusty Phillips.pdf
________________________________________
# 🚀 Criado por :
Matheus da Silva Xavier
Keven Iuri Souza dos Santos
Santiago Ramos de Lima






