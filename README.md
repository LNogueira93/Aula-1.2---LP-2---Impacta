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

tipo = input('Tipo do quarto: ')
dias = int(input('Quantidade de diárias: '))
fone = input('Usou Telefone: ')
tv = input('Usou TV: ')

valor_total = 0
if tipo == 'P':
    valor_total = dias * 160
elif tipo == 'S':
    vlor_total = dias * 110
elif tipo == 'C':
    valor_total = dias * 85
else:
    print('Tipo inválido')
    exit()

uso_fone = 0
if fone == 'S':
    uso_fone = 3

uso_tv = 0
if tv == 'S':
    uso_tv = 4

total = valor_total + uso_fone + uso_tv

print('Hospital Comunitátio')
print('Número de dias no Hospital: {}'.format(dias))
print('Tipo de quarto: {}'.format(tipo))
print('Diárias {}{}'.format("." * 13, valor_total))
print('Telefone {}{}'.format("." * 12, uso_fone))
print('Televisão {}{}'.format("." * 11, uso_tv))
print('Total {}{}'.format("." * 15, total))
