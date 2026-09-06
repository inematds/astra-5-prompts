# FALHAS

| data | o que quebrou | menor correção | prompt \| infra |
|---|---|---|---|
| 2026-09-06 | `gh repo create --push` subiu o branch como `master` (git init local sem `-b main`); a API do GitHub Pages recusou com 422 "main branch must exist" e o `--delete master` falhou por ser o default | iniciar o repo com `git init -b main` (ou `git branch -M main` antes do primeiro push); só depois ligar o Pages | infra |
| 2026-09-06 | `data-tempo` declarado de cabeça (18–22 min) ficou abaixo do cálculo da skill (palavras/200 + prática + 0,5/quiz) em 6/6 aulas | rodar o cálculo antes de escrever o tempo e propagar em 3 lugares (view, card da trilha, landing) | prompt |
