# Gerenciador de Tarefas (React + Vite)

Aplicação simples de gerenciamento de tarefas.

Descrição

- Esta aplicação permite adicionar, marcar como concluída, remover e visualizar os detalhes de tarefas.
- As tarefas são salvas no armazenamento local do navegador (localStorage) para persistência entre sessões. A lógica principal está em [`App`](src/App.jsx).
- A navegação é feita com rotas: a rota raiz exibe a lista e o formulário de criação, e a rota de detalhes mostra título e descrição de uma tarefa (veja [`main.jsx`](src/main.jsx) e [`TaskPage`](src/pages/TaskPage.jsx)).

Funcionalidades principais

- Adicionar tarefas (com título e descrição) — componente [`AddTask`](src/components/AddTask.jsx).
- Listar tarefas, alternar estado de conclusão e excluir tarefas — componente [`Tasks`](src/components/Tasks.jsx).
- Exibir detalhes de uma tarefa em página separada usando query params — [`TaskPage`](src/pages/TaskPage.jsx).
- Componentes de UI reutilizáveis: [`Title`](src/components/Title.jsx), [`Input`](src/components/Input.jsx) e [`Button`](src/components/Button.jsx).

Como rodar

1. Instale dependências:

```sh
npm install
```

2. Inicie o servidor de desenvolvimento:

```sh
npm run dev
```

O ponto de entrada da aplicação é [`index.html`](index.html) que carrega [`main.jsx`](src/main.jsx).

Principais arquivos

- [`src/App.jsx`](src/App.jsx) — lógica principal e persistência em localStorage.
- [`src/components/AddTask.jsx`](src/components/AddTask.jsx) — formulário para criar tarefas.
- [`src/components/Tasks.jsx`](src/components/Tasks.jsx) — lista e ações das tarefas.
- [`src/pages/TaskPage.jsx`](src/pages/TaskPage.jsx) — página de detalhes da tarefa.
- [`src/components/Title.jsx`](src/components/Title.jsx), [`src/components/Input.jsx`](src/components/Input.jsx), [`src/components/Button.jsx`](src/components/Button.jsx) — componentes de apresentação.
- [`package.json`](package.json) — scripts e dependências.

Notas

- O projeto usa Vite e Tailwind CSS (configuração em `tailwind.config.js`).
- Há um fetch comentado em [`App`](src/App.jsx) que pode ser usado para carregar tarefas de uma API externa.

Desenvolvido por

- Vitoria Fernandez
