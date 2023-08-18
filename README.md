# inic
cod meus 

from math import pi
import sys
cor = '\033[31m'
normal = '\033[37m'
def help():
    print(cor ,"erro", normal)
    
def circulo(raio):
    return pi * float(raio) ** 2
if __name__ == "__main__":
    if len(sys.argv) < 2:
        help()
        sys.exit(1)
    if not sys.argv[1].isnumeric():
        help()
        print("erro tem q ser numero")
        sys.exit(2)
        
        
    
    raio =sys.argv[1]
    area = circulo(raio)
    print("sbedhb", area)
    
def faixa(idade):
    if idade in range(19):
        return "menor de idade"
    elif idade in range(19,50):
        return "adulto"
    elif idade in range(50,101):
        return "velho"
    elif idade >= 100:
        return "imortal"
    else:
        return "idade invalidade"
if __name__ == "__main__":
    for idade in (-2, 19, 50, 113):
        print(f"{idade}: {faixa(idade)}")
        
def semana(dia):
    dias = {
        1: "segunda",
        2: "terca",
        3:"quarta",
        4:"quinta",
        5:"sexta",
        6: "sab",
        7:"dom"}
    return dias.get(dia, "**invalido**")



    
if __name__ == "__main__":
    for dia in range(9):
        print(f"{dia}:{semana(dia)}")


def faixa(idade):
    if idade in range(18):
        return "menor de idade"
    elif idade in range(18,51):
        return "adulto"
    elif idade in range(51,101):
        return "velho"
    elif idade >= 100:
        return "imortal"
    else:
        return "idade invalidade"
if __name__ == "__main__":
    for idade in (-2, 18, 19, 49, 50,51,100, 113,  0):
        print(f"{idade}: {faixa(idade)}")


frase = "Esta FWEFEFWEF é HUEHGRGB FERFWF umaFRF fraseEF EFRF com várias  EHBE EJWHVE EJWIH JUHE EHG"
palavras = frase.split(" ", 3)  # Dividirá em até 3 partes
print(palavras)  # Saída: ['Esta', 'é', 'uma', 'frase com várias palavras.']

"""produto = {"nome": "apple" , "preco" : 12,
           "imporatada": True , "estoq": 1 }

for cellphone in produto:
    print(cellphone)
    
for cellphone in produto.values():
    print(cellphone)

for obj, marca in produto.items():
    print(obj, "=", marca)"""
    
#for i in range(1,11):
    #if i % 3 == 0:
        #continue
    #print(i)                 
    
    
from random import randint

def sorteio():
    return randint(1,6) #sorteio

for i in range(1,7):
    if i % 2 == 1:
        continue #e para numero impar td vez q aparecer um numero q % 2 == 0 
    #ele para e passa pro outro q nao eh impar
    
    if sorteio() == i:
        print("acertou", i)
        break #tem if e else e mesmo o else estando embaixo e nao estando na mesma linha
    #ele nao executa o else se acertou o if sem o break mostraria os dois resultados
else:
    print("errou", i)   


import tkinter as tk
from tkinter import messagebox

def adicionar_tarefa():
    tarefa = entrada.get()
    if tarefa:
        lista_tarefas.insert(tk.END, tarefa)
        entrada.delete(0, tk.END)
    else:
        messagebox.showwarning("Atenção", "Digite uma tarefa!")

def remover_tarefa():
    selecionado = lista_tarefas.curselection()
    if selecionado:
        lista_tarefas.delete(selecionado)
    else:
        messagebox.showwarning("Atenção", "Selecione uma tarefa para remover!")

# Configuração da janela
janela = tk.Tk()
janela.title("Aplicativo de Lista de Tarefas")

# Entrada de tarefas
entrada = tk.Entry(janela, width=40)
entrada.pack(padx=10, pady=10)

# Botão para adicionar tarefas
botao_adicionar = tk.Button(janela, text="Adicionar Tarefa", command=adicionar_tarefa)
botao_adicionar.pack()

# Lista de tarefas
lista_tarefas = tk.Listbox(janela, width=40)
lista_tarefas.pack(padx=10, pady=10)

# Botão para remover tarefas
botao_remover = tk.Button(janela, text="Remover Tarefa Selecionada", command=remover_tarefa)
botao_remover.pack()

# Executar aplicativo
janela.mainloop()

for x in range(1,11):
    for y in range(1,11):
        print(f"{x} * {y} = {x * y}")
#DEMOREI MT TEMPO P ENTENDER ISSO AGPRA ENTEBDI MEU MUNDO EXPLODIU SE NAO ENTENDER DER PLAY
lista = ["oii","oi", "sss", "ola"]
for posicao, nome in enumerate(lista):
    #print(f"posicao: {posicao} nome : {nome}")
    print(posicao+1, nome)
for i in set("muito fixe"):
    print(i)

for i in range(1,11):
    if i % 2 == 0:
        continue
    print(i)  
for j in range(1,11):
    if j == 5:
        break
    print(j)  
        
        
