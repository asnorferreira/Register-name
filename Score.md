print('Identifique-se')
n = str(input('Digite seu nome completo: ')).strip()
nome = n.split()
print('Usuário foi identificado: {}'.format(n))

print('Selecione a sua disciplina abaixo: ')
disciplinas = ['Linguagem de progamação', 'Cálculo 2', 'Quimica 2']
disciplinas.sort()
print(disciplinas)
disciplina= str(input('Insira o nome da disciplina: '))
while True:
    try:
        lp = float(input('Digite sua nota de participação da 1 VA: '))
        if not 10 >= lp >= 0:
           print("Valor incorreto.")
           ValueError: print('Insira um numero de 0 a 10!')
           continue 
        else:
           break
    finally:
        try: 
            lp1 = float(input('Digite sua nota de atividades da 1 VA: '))
            if not 10 >= lp1 >= 0:
               print("Valor incorreto.")
               ValueError: print('Insira um numero de 0 a 10!')
               continue
            else:
               break
        finally:
            try: 
                lp2 =  float(input('Digite sua nota do projeto da 1 VA: '))
                if not 0 <= lp2 <= 10:
                   print("Valor incorreto.")
                   ValueError: print('Insira um numero de 0 a 10!')
                   continue
                else:
                   break
            finally:
                try: 
                    lp3 =  float(input('Digite sua nota de apresentação da 2 VA: '))
                    if not 0 <= lp3 <= 10:
                       print("Valor incorreto.")
                       ValueError: print('Insira um numero de 0 a 10!')
                       continue
                    else:
                       break
                finally:
                    try:
                        lp4 =  float(input('Digite sua nota de atividades da 2 VA: '))
                        if not 0 <= lp4 <= 10:
                           print("Valor incorreto.")
                           ValueError: print('Insira um numero de 0 a 10!')
                           continue
                        else:
                           break
                    finally:
                        try:
                            lp5 =  float(input('Digite sua nota do projeto da 2 VA: '))
                            if not 0 <= lp5 <= 10:
                               print("Valor incorreto.")
                               ValueError: print('Insira um numero de 0a 10!')
                               continue
                            else:
                               break
                        finally:
                            break

print()                      
print('Média na 1 VA: ', ((lp*2) + (lp1*4) + (lp2*4))/ 10)
print('Média na 2 VA: ', ((lp3*2) + (lp4*3) + (lp5*5))/ 10)
fVA = float((lp * 2) + (lp1 * 4) + (lp2 * 4)) / 10
sVA = float((lp3 * 2) + (lp4 * 4) + (lp5 * 4))/ 10
print('A média respectiva é de: ', ((fVA) + (sVA)) / 2)
charque = ((fVA) + (sVA)) / 2

if charque >= 7:
   print('Aprovado.')
if charque < 3:
   print('Reprovado.')
if 7 < charque >= 3 :
    while True:
        try:
            zVA = float(input('Digite sua nota total da 3 VA: '))
            if not 10>= zVA >=0:
                ValueError: print('Insira um numero de 0 a 10!')
                continue
            else:
                break
        finally:
            break

print()
nota = [fVA, sVA, zVA]
NotaMaior = max(nota)
nota.remove(max(nota))
NotaMediana = max(nota)
print(NotaMaior)
print(NotaMediana)
print('MÉDIA: ', ((NotaMaior) + (NotaMediana)) / 2)
final = ((NotaMaior) + (NotaMediana)) / 2
if final > 5:
   print('Aprovado por nota.')
if final < 5:
   print('Reprovado.')
print()
