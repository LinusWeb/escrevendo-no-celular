# 2o Plano de teste - Escrevendo no celular
### Membros: 
- Juscelino Messias
- Emmanuel Bulacio

### Problema:
http://dojopuzzles.com/problemas/exibe/escrevendo-no-celular/

### Tecnologias: 
- Linguagem de programação:
  - Java
- SO:
  - Linux (Debian 8.x release Jessie) 
  - Windows 10
- Ambiente de produção:  
  - Netbeans IDE 8.2  
- Ferramenta de Testes:
  - JUnit 4.12  
 
# Descrição:
Letras | Numero de dominio
:-----: | :------:
ABC    |  2 
DEF    |  3 
GHI    |  4 
JKL    |  5 
MNO    |  6 
PQRS    |  7 
TUV    |  8 
WXYZ   |  9 
Espaço | 0 

Desenvolva um programa que, dada uma mensagem de texto limitada a 255 caracteres, retorne a seqüência de números que precisa ser digitada. Uma pausa, para ser possível obter duas letras referenciadas pelo mesmo número, deve ser indicada como _.

# Exemplo
"SEMPRE ACESSO O DOJOPUZZLES" é equivalente á sequencia 77773367_7773302_222337777_777766606660366656667889999_9999555337777
Sendo que para representar uma letra dentro do dominio de um numero esse numero deve ser informado segundo o numero da posição da letra desejada dentro do dominio.


# Plano de teste

Entrada | Condição | Classes Válidas | Classes Inválidas
:-----: | :------: | :-------------: | :---------------:
  text  | text é do tipo String  text caracteres ]'A','Z']  | text caracteres são letras ou espaço | text tem caracteres numericos ou especiais 
  
def is_valid(text):
  return True;
  
 InstanceOf("Ola mundo")==String
 
 def getTextNumbers(text):
    is_valid(text);
    return String;

## 1º caso de teste

is_valid("Ola mundo") == true

getTextNumbers("Ola mundo") == String processada

## 2º caso de teste
is_valid("Feliz 2017") == false

getTextNumbers("Feliz 2017")  # Isso aqui lança uma exceção

## 3º caso de teste
 is_valid(18)  # Isso aqui lança uma exceção
 
 getTextNumbers(18)  # Isso aqui lança uma exceção

## 4º caso de teste
is_valid("       ") == true

getTextNumbers("       ") == String processada (0000000)
