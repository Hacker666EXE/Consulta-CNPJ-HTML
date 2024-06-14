# Consulta de CNPJ

Este é um aplicativo web simples desenvolvido em HTML, CSS e JavaScript para consultar informações de empresas através do CNPJ utilizando a API da ReceitaWS.

## Funcionalidades

- **Formulário de Consulta**: Permite ao usuário inserir um CNPJ válido para consultar as informações da empresa correspondente.
  
- **Requisição à API**: Ao enviar o formulário, o JavaScript captura o CNPJ digitado, realiza uma requisição à API da ReceitaWS através de um proxy (`https://api.allorigins.win/raw?url=`), e exibe os dados da empresa na página.

- **Exibição de Dados**: Os dados da empresa são exibidos em um formato estruturado dentro de um cartão (`<div>` com classe `card`), incluindo nome, CNPJ, data de abertura, situação cadastral, tipo, porte, natureza jurídica, atividade principal, endereço completo, telefone, data da última atualização e quadro de sócios e administradores.

- **Tratamento de Erros**: Caso haja algum problema na requisição à API ou se o CNPJ inserido não for válido, uma mensagem de erro é exibida na interface.

## Estrutura do Código

- **HTML**: Define a estrutura básica da página, incluindo o formulário de consulta e a área para exibir os resultados da consulta.

- **CSS**: Aplica estilos visuais à página para garantir uma experiência de usuário agradável, utilizando cores, fontes e espaçamentos adequados.

- **JavaScript**: Controla o comportamento dinâmico da página, validando o CNPJ inserido, fazendo a requisição à API de forma assíncrona, tratando os dados recebidos e exibindo-os na interface de usuário.

## Como Utilizar

1. **Clone o Repositório**: Baixe ou clone os arquivos `index.html`, `styles.css` e `script.js` para o seu ambiente local.

2. **Abra o Arquivo HTML**: Abra o arquivo `index.html` em um navegador web (Chrome, Firefox, etc.).

3. **Consulta de CNPJ**:
   - Insira um CNPJ válido no campo de entrada.
   - Clique no botão "Consultar" para ver as informações da empresa na área destacada.

## Observações

- Este aplicativo utiliza um proxy (`https://api.allorigins.win/raw?url=`) para contornar problemas de política de mesma origem (CORS) ao acessar a API da ReceitaWS diretamente do navegador.
  
- Certifique-se de ter uma conexão com a internet ativa para realizar consultas válidas à API.

Este projeto foi criado para demonstrar como integrar APIs externas em páginas web usando JavaScript e oferecer uma interface simples e eficiente para consultar informações de empresas através do CNPJ.
  ![checker cnpj](cnpj.png)