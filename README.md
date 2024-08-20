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
cv=int(l[8])
soma=0
for n in l:
    num=int(n)
    soma=num+soma
div=soma%11
if cpft<9:
    print("CPF Inválido")
elif div!=0:
    print("CPF Inválido")
elif uf!=cv:
    print("CPF Inválido")
else:
    print("CPF Válido")
