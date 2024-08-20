'''

Welcome to GDB Online.
GDB online is an online compiler and debugger tool for C, C++, Python, Java, PHP, Ruby, Perl,
C#, OCaml, VB, Swift, Pascal, Fortran, Haskell, Objective-C, Assembly, HTML, CSS, JS, SQLite, Prolog.
Code, Compile, Run and Debug online from anywhere in world.

'''
cpf=input("Digite o seu CPF sem pontos ou traços:")
uf=int(input("""Digite o codigo da UF onde seu cpf foi cadastrado:
Código 0:  Rio Grande do Sul    
Código 1:  Distrito Federal – Goiás – Mato Grosso – Mato Grosso do Sul – Tocantins    
Código 2:  Pará – Amazonas – Acre – Amapá – Rondônia – Roraima    
Código 3:  Ceará – Maranhão – Piauí    
Código 4:  Pernambuco – Rio Grande do Norte – Paraíba – Alagoas    
Código 5:  Bahia – Sergipe    
Código 6:  Minas Gerais    
Código 7:  Rio de Janeiro – Espírito Santo
Código 8:  São Paulo
Código 9: Paraná – Santa Catarina
"""
))
cpft=len(cpf)
l=list(cpf)
cv=l[8]
soma=0
for n in l:
    num=int(n)
    soma=num+soma
div=soma%11
if cpft<9:
    print("CPF Inválido4")
elif div!=0:
    print("CPF Inválido3")
elif uf!=cv:
    print("CPF Inválido2")
else:
    print("CPF Válido1")

