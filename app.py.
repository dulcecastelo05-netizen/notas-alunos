nome = input ("Nome do aluno: ")
print ("Aluno:",nome)
nota1 =float(input("Nota da prova 1: "))
nota2 =float(input("Nota da prova 2: "))
nota3 =float(input("Nota da prova 3: "))
media = (nota1 + nota2 + nota3) /3
print("Média:", media)
if media >= 10:
    resultado = "Aprovado"
elif media >= 7:
    resultado = "Recuperação"
else:
    resultado = "Reprovado"
print("Resultado:", resultado)
alunos = []
aluno = {"nome": nome, "media": media, "resultado": resultado}
nota_maxima = 20
nota_aprovacao = 10
nota_recuperacao = 7

alunos = []

while True:
    nome = input("Nome do aluno (escreva fim para terminar): ")
    if nome == "fim":
        break

    nota1 = float(input("Nota da prova 1: "))
    nota2 = float(input("Nota da prova 2: "))
    nota3 = float(input("Nota da prova 3: "))

    media = (nota1 + nota2 + nota3) / 3

    if media >= nota_aprovacao:
        resultado = "Aprovado"
    elif media >= nota_recuperacao:
        resultado = "Recuperação"
    else:
        resultado = "Reprovado"

    aluno = {"nome": nome, "media": media, "resultado": resultado}
    alunos.append(aluno)

print("Lista de alunos")
for aluno in alunos:
    print(aluno["nome"], "-", aluno["media"], "-", aluno["resultado"])
    if len(alunos) > 0:
        soma = 0
    maior = alunos[0]["media"]
    menor = alunos[0]["media"]
    aprovados = 0

    for aluno in alunos:
        soma = soma + aluno["media"]
        if aluno["media"] > maior:
            maior = aluno["media"]
        if aluno["media"] < menor:
            menor = aluno["media"]
        if aluno["resultado"] == "Aprovado":
            aprovados = aprovados + 1

    media_turma = soma / len(alunos)

    print("Total de alunos:", len(alunos))
    print("Média da turma:", round(media_turma, 1))
    print("Maior média:", round(maior, 1))
    print("Menor média:", round(menor, 1))
    print("Aprovados:", aprovados)
    nota_maxima = 20
nota_aprovacao = 10
nota_recuperacao = 7


def calcular_media(n1, n2, n3):
    return (n1 + n2 + n3) / 3


def classificar(media):
    if media >= nota_aprovacao:
        return "Aprovado"
    elif media >= nota_recuperacao:
        return "Recuperação"
    else:
        return "Reprovado"


alunos = []

while True:
    while True:
     nome = input("Nome do aluno (escreva fim para terminar): ")
    if nome == "fim":
        break

    nota1 = ler_nota("Nota da prova 1: ")
    nota2 = ler_nota("Nota da prova 2: ")
    nota3 = ler_nota("Nota da prova 3: ")

    media = calcular_media(nota1, nota2, nota3)
    resultado = classificar(media)

    aluno = {"nome": nome, "media": media, "resultado": resultado}
    alunos.append(aluno)
