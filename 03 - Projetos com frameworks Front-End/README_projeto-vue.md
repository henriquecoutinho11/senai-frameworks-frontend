# Pausa

Uma lista de tarefas simples para organizar o dia com mais leveza. Adicione o que precisa ser feito, acompanhe o progresso e mantenha o foco no que importa.

## Recursos

- Adicionar novas tarefas
- Marcar tarefas como concluídas
- Filtrar tarefas por status: todas, pendentes ou concluídas
- Remover tarefas
- Salvar automaticamente a lista no navegador com `localStorage`
- Exibir o progresso das tarefas concluídas

## Tecnologias

- [Vue 3](https://vuejs.org/)
- [TypeScript](https://www.typescriptlang.org/)
- [Vite](https://vite.dev/)

## Requisitos

- Node.js `22.18+` ou `24.12+`
- npm

## Instalação

Clone o projeto, entre na pasta e instale as dependências:

```bash
npm install
```

## Desenvolvimento

Inicie o servidor local com recarregamento automático:

```bash
npm run dev
```

O endereço local será exibido no terminal, normalmente `http://localhost:5173`.

## Comandos disponíveis

| Comando              | Descrição                                                  |
| -------------------- | ---------------------------------------------------------- |
| `npm run dev`        | Inicia o servidor de desenvolvimento                       |
| `npm run type-check` | Verifica os tipos TypeScript e Vue                         |
| `npm run build`      | Executa a verificação de tipos e gera a versão de produção |
| `npm run preview`    | Serve localmente o build de produção                       |

## Estrutura principal

```text
src/
├── App.vue              # Interface e lógica da lista de tarefas
├── main.ts              # Inicialização da aplicação
└── assets/
    ├── base.css         # Estilos base
    └── main.css         # Estilos da aplicação
```

## Produção

Gere os arquivos otimizados para produção:

```bash
npm run build
```

Os arquivos serão gerados na pasta `dist/`.
