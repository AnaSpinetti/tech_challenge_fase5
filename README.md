# Visão Geral do Projeto

## Swagger da API: https://documenter.getpostman.com/view/16258060/2sA3XQiNas

A aplicação foi criada para permitir que o usuário logado possa realizar o gerenciamento de seu time e as tarefas a serem realizadas. As tarefas são atribuídas ao usuário responsável pela execução. É possível também gerenciar a carga horária dos membros do time.

## Tecnologias Utilizadas
- **Front-end**: React.js e SASS para estilização
- **Back-end**: Node.js com Express.js
- **Banco de Dados**: Firestore
- **Autenticação**: Firebase

***Nota***: Não foi possível utilizar o Firebase Cloud Functions para notificações, devido a mensagem na página informando que seria necessário realizar um upgrade do plano.

## Configuração do Ambiente

### Pré-requisitos
- Node.js
- NPM

### Execução da Aplicação

#### Backend
1. Descompacte a pasta do projeto.
2. Abra o CMD no caminho correspondente à pasta `backend`.
3. Realize a instalação das dependências necessárias com o comando:
```bash
    npm install
```
4. Após instalar as dependências, a pasta node_modules será criada.
5. Execute o backend com o comando:
```bash
    node index.js
```

#### Frontend
1. Após isso vamos subir o frontend. Abra o CMD no caminho correspondente a pasta frontend
2. Realize a instalação das dependências necessárias para a execução do projeto com o comando:
```bash
    npm install
```
3. Após instalar as dependências, poderá ver que a pasta node_modules foi criada.
4. Execute então o frontend com o comando:
```bash
    npm start
```
5. ainda no caminho raiz da pasta frontend. Valide a porta em que a aplicação foi iniciada, a porta configurada para o projeto é a porta 3000.
6. O navegador com a tela inicial da aplicação será aberta automaticamente, caso não seja, abra seu navegador e acesse localhost:3000


A tela de login está integrada com o Firebase Authenticator, para realizar login crie um novo usuário com a opção "Cadastre-se"
No dashboard são exibidos todos os membros do time e as tarefas cadastradas pelo responsável pelo sistema, nessa tela podemos cadastrar novos membros ao time e novas tarefas. Também podemos editar ou excluir os dados cadastrados.
Ao clicar no ícone de edição de tarefas ou membros, os componentes de edição são exibidos com as informações atuais pré-preenchidas
Ao clicar no ícone de exclusão (lixeira) é feita a chamada para a API correspondente ao método delete (vide swagger do backend)
