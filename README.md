# Sistema-de-Gerenciamento-de-Livros
Trabalho final da matéria de Algoritmo e Estrutura de Dados I, do primeiro período do curso de Ciência da Computação.

**1. Descrição:**

Neste trabalho, voce devera criar um pequeno sistema para gerenciamento de livros de uma biblioteca ou livraria. Seu sistema devera, obrigatoriamente, ser baseado no pequeno trecho de codigo abaixo:

#include <stdio.h>

void listar();

void inserir(char ∗ titulo, char ∗ autor, int num paginas);

void remover(char ∗ titulos);

int buscar(char ∗ titulo);

Abaixo, segue a definicao das funcoes que deverao ser implementadas em seu codigo e o detalhamento do que um livro devera conter:

**Livro:** Um livro devera conter tres campos:

• Tıtulo
• Nome do autor
• Numero de paginas

O tıtulo e o nome do autor deverao ser strings. Ja o numero de paginas devera ser um inteiro maior ou igual a zero.

**Menu:** A base do sistema devera ser um menu que contem 5 opcoes:
1. Inserir livro
2. Remover livro
3. Buscar livro
4. Listar livros
5. Sair

O usuario podera escolher uma das opcoes (de 1 a 5) e realizar a operacao desejada. Este menu devera ser mostrado de forma repetida ate que o usuario escolha a opcao sair.

**Listar:** Esta funcao devera exibir na tela, de forma clara e organizada, todos os livros da base de dados. Para cada livro, devera ser exibido todos os seus dados (nome do livro, nome do autor e numero de paginas). Alem disso, esta listagem devera ser realizada em ordem alfabetica do tıtulo dos livros.

**Inserir:** Devera ser inserido um novo livro no sistema. A funcao inserir devera receber os tres campos(tıtulo, nome do autor e numero de paginas). Esta funcao nao devera permitir a insercao de livros com tıtulos duplicados. Isto e, no momento da insercao, devera ser realizada uma busca pelo tıtulo na base de dados. Caso o livro ja conste na base, este nao devera ser inserido e uma mensagem de erro devera ser retornada ao usuario.

**Remover:** Esta funcao devera remover um livro da base de dados. Ela devera, incialmente, buscar o tıtulo do livro na base. Caso o livro exista, ele devera ser removido e o usuario devera ser alertado sobre a remocao com sucesso. Caso o livro nao exista, devera ser exibida uma mensagem para o usuario que o livro nao pode
ser removido, pois o tıtulo digitado nao existe na base de dados.

**Buscar:** Realiza uma consulta sobre a existencia ou nao de um livro na base de dados. Caso o livro exista, entao devera ser exibido, na tela, todos os dados referentes a aquele livro (tıtulo, nome do autor e numero de paginas). Caso o livro nao exista, devera ser exibida uma mensagem de erro para o usuario.

**2 Restricoes:**
Algumas restricoes deverao ser observadas no desenvolvimento deste trabalho:

1. Ao utilizar a funcao Exibir, os livros deverao ser mostrados ao usuario na ordem alfabetica de seus tıtulos.

2. O sistema devera ser persistente. Isto e, a base de dados devera ser salva em disco, com o uso de arquivos. Quando o sistema e reaberto, esta base de dados e adquirida e o usuario consegue continuar com a utilizacao normal do sistema.

3. Erros nos inputs deverao ser tratados corretamente. Desta forma, voce devera sempre verificar se o usuario nao entrou com dados indevidos. Exemplos de inputs indevidos sao uma opcao invalida no menu ou a utilizacao de uma string para representar o numero de paginas de um livro.
