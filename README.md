# Tô nos Cursos

Aplicação em React + Vite com duas páginas (Início e Cadastro), navegação com React Router e formulário com validação. Atividade avaliativa de Aplicativos Web — IFTO, Campus Palmas.

Aluno: SEU NOME AQUI
Turma: SUA TURMA AQUI

## Como executar

```bash
npm install
npm run dev
```

Abra o endereço mostrado no terminal (geralmente http://localhost:5173).

## Estrutura

```
src/
  pages/
    Inicio.jsx
    Cadastro.jsx
  App.jsx
  App.css
  main.jsx
```

## Como funciona

A navegação usa o React Router: o `BrowserRouter` envolve o `App` em `main.jsx`, e o `App.jsx` define as rotas com `Routes` e `Route`, usando `NavLink` no menu para trocar de página sem recarregar o site. Uma rota `*` mostra "Página não encontrada" para endereços inexistentes. O formulário é controlado com `useState`: cada campo é atualizado pelo `onChange`, e no envio o `preventDefault()` evita o recarregamento. A função `validar()` retorna um objeto com os erros de cada campo, e o cadastro só é confirmado quando esse objeto está vazio, momento em que a mensagem de sucesso aparece e o formulário é limpo.

## Personalizações do desafio

- Nome da aplicação "Tô nos Cursos" e tema em bege e roxo.
- Campo "Curso de interesse" (select) com três opções, obrigatório na validação e limpo após o envio.
- Frase de orientação própria na página Início e mensagem de sucesso personalizada com nome e curso.

## Testes realizados

Os prints estão na pasta `prints/`:

1. `1-inicio.png` — página Início
2. `2-cadastro.png` — página Cadastro
3. `3-erros.png` — erros de validação
4. `4-sucesso.png` — mensagem de sucesso

## Observação

Os dados não são enviados a nenhuma API nem salvos em banco de dados: ficam apenas no estado do React e somem ao atualizar a página.
