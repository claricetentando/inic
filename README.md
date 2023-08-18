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
        
        
