O Modelo de Entidade-Relacionamento (MER) é usado para representar visualmente as entidades de dados, atributos de entidades e as relações entre elas em um banco de dados. Ele ajuda a compreender a estrutura do banco de dados.

Existem três tipos principais de relacionamentos:
Relações 1x1 (um para muitos): Isso significa que uma entidade em uma tabela se relaciona exatamente com uma entidade na outra.

Relações 1xN (um para muitos): Isso significa que uma entidade em uma tabela está associada a várias entidades em outra tabela. É o tipo mais comum de relação.

Relações NxN (muitos para muitos): Este tipo de relação indica que muitas entidades em uma tabela estão associadas a muitas entidades em outra tabela. Isso geralmente é resolvido através da criação de uma terceira tabela, chamada de tabela de junção ou tabela intermediária, que mapeia os relacionamentos entre as duas tabelas. 

## Aplicando os relacionamentos:

### 1 - "forms":
  Não há relações explícitas nesta tabela.

### 2 - "fields":
  Tem uma relação 1xN com a tabela "forms", indicando que um formulário pode ter vários campos. Isso é representado pela coluna "id_forms" que referencia a coluna "id" da tabela "forms".

### 3 - "users":
Não há relações explícitas nesta tabela.

### 4 - "fieldOptions": 
Não há relações explícitas nesta tabela.

### 5 - "answerFields":
Tem uma relação 1xN com a tabela "fields", indicando que um campo pode ter várias respostas. Isso é representado pela coluna "id_fields" que referencia a coluna "id" da tabela "fields".
Também tem uma relação 1xN com a tabela "answers", indicando que uma resposta pode ter vários campos respondidos. Isso é representado pela coluna "id_answers" que referencia a coluna "id" da tabela "answers".

### 6 - "answers":
Tem uma relação 1xN com a tabela "fields", indicando que uma resposta pode estar associada a vários campos. Isso é representado pela coluna "id_fields" que referencia a coluna "id" da tabela "fields".
