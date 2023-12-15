# 20232BSET03P2
Inteli - Engenharia de Software | Avaliação 2023-2B P2

## vulnerabilidades identificadas

- Na rota de post para adicionar um voto a algum animal, não estávamos validados para ver se aquele animal realmente existia na tabela. Foi adicionada essa verificação
- Na rota de post para criar um gato era possível realizar um SQL Injection, uma vez que o valor para o nome do gato estava utilizando uma concatenação de strings para o nome ficar entre ''. Foi então adicionado na rota que valor do nome fosse passado como um parâmetro na consulta SQL.
- O tratamento de erro antes poderia fazer o vazamento de dados sensíveis para o usuário, então foi adicionado com tratamento de erros com mensagens simples que não possuem informações críticas da aplicação.
- A criação do banco de dados estava errada, onde os tipos das colunas foram modulados e agora a coluna ID é uma PRIMARY KEY.

