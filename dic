from cardapioOriginal import *

def ex2():
    soma = 0
    for cidx, c in categorias.items():
        soma = soma + len(c)
    print("Numero de pratos: " + str(soma))
    # ou len(pratos)

def ex3():
    pizza = {"n": "Vai de tudo", "i": [], "p": 0.0}
    for i in ingredientes:
        pizza["i"].append(i)

    novoPratoIdx = list(pratos)[-1] + 1
    pratos[novoPratoIdx] = pizza

    categorias["Pizzas"].append(novoPratoIdx)

def ex4():
    primeiraCategoria = list(categorias)[0]
    pratos[categorias[primeiraCategoria][0]]["p"] = 12.34
    #ou pratos[0]["p"] = 12.34

def ex5():
    for idx, prato in pratos.items():
        print(prato["n"])

def ex6():
    #nomes dos pratos repetem -> gambiarra
    novoDict = {}
    for cidx, cat in categorias.items():
        for prato in cat:
            tempArr = []
            for ing in pratos[prato]["i"]:
                tempArr.append(ingredientes[ing])
            novoDict[cidx + ":" + pratos[prato]["n"]] = tempArr
    return novoDict

def ex7(dict):
    dictIngredientes = {}
    for idx, prato in dict.items():
        for ing in prato:
            dictIngredientes[ing] = dictIngredientes[ing] + 1 if ing in dictIngredientes else 1


ex2()
ex3()
ex4()
ex5()
dictEx6 = ex6()
ex7(dictEx6)
