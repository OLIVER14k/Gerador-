import random
import string

def gerar_senhas(tamnho=12):
    caracteres = string.ascii_letters + string.digits + string.punctuation
    senha = ''.join(random.choice(caracteres) for _ in range(tamnho) )
    return senha
 
tamanho_da_senha = int(input("digite o tamnho da senha desejada: "))
for i in range(10):
    senha_gerada = gerar_senhas(tamanho_da_senha)   
    print("senha_gerada:", senha_gerada)  
