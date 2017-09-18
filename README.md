# 2o Plano de teste - Escrevendo no celular
### Membros: Juscelino Messias / Emmanuel Bulacio
### Problema: http://dojopuzzles.com/problemas/exibe/escrevendo-no-celular/
### Tecnologia: Java

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
  text  | text é do tipo String  | text caracteres são letras ou espaço | text tem caracteres numericos ou especiais
  09    |    10    |        11       |         12
  13    |    14    |        15       |         16
  17    |    18    |        19       |         20  


## 1º caso de teste
teste

## 2º caso de teste
teste

## 3º caso de teste
teste

## 4º caso de teste
teste

## 5º caso de teste
teste
