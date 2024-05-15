# L-gica.py
notas = []

def adicionar_nota(nota):
    notas.append(nota)
    atualizar_lista_notas()
    calcular_media()

def atualizar_lista_notas():
    lista_notas = []  # Não há uma representação direta de HTML em Python, então usaremos uma lista simples para representar as notas
    for nota in notas:
        lista_notas.append(nota)
    imprimir_lista_notas(lista_notas)

def imprimir_lista_notas(lista_notas):
    print("Lista de Notas:")
    for nota in lista_notas:
        print(nota)

def calcular_media():
    somatorio_notas = sum(notas)
    media = somatorio_notas / len(notas)

    if media > 6:
        print(f"Média: {media:.2f} - Pessoa estudante APROVADA")
    else:
        print(f"Média: {media:.2f} - Pessoa estudante REPROVADA")

# Exemplo de utilização
adicionar_nota(7)
adicionar_nota(8)
adicionar_nota(5)
