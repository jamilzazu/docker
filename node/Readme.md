# Nginx com Node.js

A idéia principal é que quando um usuário acesse o nginx, o mesmo fará uma chamada em nossa aplicação node.js. Essa aplicação por sua vez adicionará um registro em nosso banco de dados mysql, cadastrando um nome na tabela people.

O retorno da aplicação node.js para o nginx deverá ser: Full Cycle Rocks! e uma lista de nomes cadastrada no banco de dados.

1. Clonar este repositório
2. Acessar a pasta raiz do projeto e executar no terminal `docker-compose up -d --build`
3. Acessar via navegador http://localhost:8080/