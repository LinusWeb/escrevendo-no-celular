# 2o Plano de teste - Escrevendo no celular
### Membros: 
- Emmanuel Bulacio
- Juscelino Messias

### Link para o problema:
http://dojopuzzles.com/problemas/exibe/escrevendo-no-celular/
 
### Descrição:

Um dos serviços mais utilizados pelos usuários de aparelhos celulares são os SMS (Short Message Service), que permite o envio de mensagens curtas (até 255 caracteres em redes GSM e 160 caracteres em redes CDMA).

Para digitar uma mensagem em um aparelho que não possui um teclado QWERTY embutido é necessário fazer algumas combinações das 10 teclas numéricas do aparelho para conseguir digitar. Cada número é associado a um conjunto de letras como a seguir:

Letras | Numero de dominio
:----: | :----:
ABC    |  2 
DEF    |  3 
GHI    |  4 
JKL    |  5 
MNO    |  6 
PQRS   |  7 
TUV    |  8 
WXYZ   |  9 
Espaço |  0 

Desenvolva um programa que, dada uma mensagem de texto limitada a 255 caracteres, retorne a seqüência de números que precisa ser digitada. Uma pausa, para ser possível obter duas letras referenciadas pelo mesmo número, deve ser indicada como _.

### Exemplo:
"SEMPRE ACESSO O DOJOPUZZLES" é equivalente á sequencia 77773367_7773302_222337777_777766606660366656667889999_9999555337777
Sendo que para representar uma letra dentro do dominio de um numero esse numero deve ser informado segundo o numero da posição da letra desejada dentro do dominio.

### Tecnologias: 
- Linguagem de programação:
  - Java 8 Update 141
- SO:
  - Linux (Debian 8.x release Jessie) 
  - Windows 10
- Ambiente de produção:  
  - Netbeans IDE 8.2  
- Ferramenta de Testes:
  - JUnit 4.12  

# Plano de teste

Entrada | Condição | Classes Válidas | Classes Inválidas
:-----: | :------: | :-------------: | :---------------:
  text  | text é do tipo String  text caracteres ]'A','Z']  | text caracteres são letras ou espaço | text tem caracteres numericos ou especiais 
  text  | qtdCaracteres(text) <= 255 | qtdCaracteres(text) < 256 | qtdCaracteres(text) > 255
  
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

## 5º caso de teste (text excede 255 caracteres)
is_invalid("text text text text text...") # Isso aqui lança uma exceção
