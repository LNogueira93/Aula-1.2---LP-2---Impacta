# Aula-1.2---LP-2---Impacta

Um hospital precisa de um programa para calcular e imprimir os gastos de um
paciente. A tabela de preços do hospital é a seguinte:

Quartos (diária):
Particular – R$ 160,00
Semi-particular – R$ 110,00
Coletivo – R$ 85,00

Telefone (uso): R$ 3,00
Televisão (uso): R$ 4,00

Escreva um programa em Python que leia: o número de dias gastos no hospital; um
caractere representando o tipo do quarto (P, S, C); um caractere indicando se usou ou
não o telefone (S, N); outro caractere indicando se usou ou não a televisão (S, N).
Então emita o seguinte relatório:

Hospital Comunitário
Número de dias no hospital: 6
Tipo de quarto: P
Diárias.............960.0
Telefone............0.0
Televisão...........0.0
Total...............960.0


# 1800182 - Jady Pelisari Redini
# 1800180 - Lucas Moises Nogueira

dias = int(input("Quantos dias foram gastos? "))
quarto = input("Qual tipo de quarto usado? (P,S,C) ")
telefone = input("Usou o telefone? (S/N) ")
tv = input("Usou a TV? (S/N) ")

P = int(160)
S = int(110)
C = int(85)
#telefone = input("S,N")
#tv = input("S,N")

if (dias > 0):
  calc1 = int(dias * P)
  print("Hospital Comunitário")
  print("Número de dias no hospital: ",dias)
  print("Diárias...........",calc1)

#if (telefone == "S"):
#  calc2 = 3
#elif (telefone == "N"):
#  calc2 = 0
  print("Telefone...........",0)
  print("Televisão...........",0)
#total = calc1 + calc2
  print("Total...........",calc1)
