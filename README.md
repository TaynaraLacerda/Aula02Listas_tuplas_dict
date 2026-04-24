A Base de Tudo: Indexação Zero
Para o Python, uma string não é apenas um bloco de texto, mas uma sequência de
caracteres guardada em "endereços" numerados. No mundo da programação, a contagem
dessas caixas sempre começa do zero.

Exemplo Visual: String "MARIA"
Letra M A R I A

Índice (Index) 0 1 2 3 4

Alerta de Erro: Se você tentar acessar o índice 5 na palavra "MARIA", o Python
retornará o erro IndexError: string index out of range, pois a contagem termina no
4.

Acesso Individual e Slicing
Podemos capturar partes do texto de forma cirúrgica ou em lote.
2.1. Acesso Individual
Utilizamos colchetes [] para capturar uma única letra.
● nome[0] → Retorna a primeira letra.
● nome[4] → Retorna a quinta letra.
(Fatiamento)
A sintaxe utilizada é [início:fim]. Regra de Ouro: O índice de "fim" é exclusivo (o Python
corta antes dele).

● Extração com Início e Fim: nome[0:3] (Pega os índices 0, 1 e 2. O 3 fica de fora).
● Extração até o Final: nome[2:] (Começa no índice 2 e pega tudo o que sobrar).
3. Métodos Essenciais de Limpeza e Preparação
Antes de fatiar, muitas vezes precisamos "limpar" os dados que vêm do usuário.
Método Ação (O que faz) Exemplo Prático

strip() Remove espaços extras no início e no fim. texto.strip()

replace() Substitui um caractere/texto por outro. cpf.replace(".", "")

lower() Converte tudo para minúsculas. email.lower()

upper() Converte tudo para maiúsculas. nome.upper()

len() Conta a quantidade total de caracteres. len(senha)

Estudo de Caso: Limpeza de CPF
A limpeza de dados garante que informações de diferentes fontes sejam padronizadas.

None
cpf = "123.456.789-00"
cpf = cpf.replace(".", "") # Remove pontos
cpf = cpf.replace("-", "") # Remove o traço
print(cpf) # Saída: 12345678900
