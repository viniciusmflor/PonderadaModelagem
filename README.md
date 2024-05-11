# PonderadaModelagem
 ponderada cristiano semana 3

Um banco de dados relacional é um tipo de sistema de banco de dados que organiza dados em tabelas, ou relações, que podem ser interconectadas por meio de chaves. Cada tabela é composta por linhas (também conhecidas como registros) e colunas (também conhecidas como atributos). A principal característica de um banco de dados relacional é a sua capacidade de eficientemente recuperar dados de várias tabelas através do uso de operações como JOINs, que permitem combinar dados de duas ou mais tabelas com base em condições relacionadas a suas chaves.
Os elementos chave de um banco de dados relacional incluem:

Tabelas: Coleções de dados organizados em um formato tabular com linhas e colunas.
Chave Primária (Primary Key, PK): Uma coluna ou grupo de colunas que identifica de maneira única cada linha em uma tabela.
Chave Estrangeira (Foreign Key, FK): Uma coluna ou grupo de colunas em uma tabela que referencia a chave primária de outra tabela, estabelecendo uma relação entre as tabelas.
Índices: Estruturas de dados que melhoram a velocidade de recuperação de dados das tabelas.
Views: Representações virtuais de um subconjunto dos dados da tabela.
Procedimentos armazenados (Stored Procedures): Scripts SQL que são armazenados no servidor de banco de dados e podem ser executados para realizar operações complexas.
Transações: Sequências de operações de banco de dados que são tratadas como uma única unidade lógica de trabalho.
Agora, olhando para a estrutura do seu banco de dados na imagem enviada:

Existem quatro principais tabelas: Instituição, Voluntariado, User e Post, com conexões entre elas indicadas por linhas, que representam relações (normalmente chaves estrangeiras).

Tabelas e Relacionamentos
Instituição

Armazena informações sobre instituições, incluindo descrição, horas de trabalho, avaliações, e outras informações.
Tem uma relação com a tabela User através de voluntariados (id) e permissoes.
Voluntariado

Contém detalhes sobre diferentes atividades de voluntariado, como nome, descrição e horas.
Relaciona-se com a tabela User através de Users (id).
User

Mantém registros de usuários, incluindo informações pessoais e atividades de voluntariado.
Conecta-se a Instituição e Voluntariado através de várias chaves estrangeiras.
Conecta-se também com Post e comentario por meio de posts e informações como foto de perfil (id) e nome fantasia.
Post

Guarda detalhes sobre posts feitos pelos usuários, incluindo data, hora, descrição e comentários.
Tem uma relação direta com comentario.
Comentario

Armazena comentários em posts específicos, relacionando-se com Post através de Nome fantasia.
Funcionamento
Os dados são armazenados de forma que as informações relevantes sobre usuários, instituições e atividades de voluntariado possam ser facilmente acessadas e gerenciadas. Por exemplo, um usuário pode fazer parte de várias atividades de voluntariado, e isso é gerenciado através das chaves estrangeiras que conectam as tabelas User e Voluntariado. As atividades e interações dos usuários são registradas em Post e Comentario, permitindo um rastreamento eficiente da comunicação e interação dentro do sistema.

Essa estrutura favorece a organização, a recuperação eficiente de informações relacionadas e a integridade dos dados, aspectos essenciais em qualquer sistema que lide com múltiplos usuários e relações complexas.






