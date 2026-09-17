# Sistema Applause

Sistema interno da Applause Formaturas: um conjunto de painéis em HTML puro (sem build, sem framework) usados para acompanhamento de vendas e checklist de solenidades de formatura.

## Arquivos

- **`index.html`** — Página inicial / menu do sistema, com login. Ponto de entrada que dá acesso aos demais painéis.
- **`painel_vendas_publico.html`** — Painel de vendas.
- **`painel_checklist.html`** — Checklist de solenidade por evento.

Os três arquivos ficam na raiz do repositório porque se referenciam entre si por links relativos (ex.: `index.html` linka para `painel_vendas_publico.html` e `painel_checklist.html`).

## Backend

O backend é o [Supabase](https://supabase.com), usado tanto como banco de dados quanto para autenticação. O login é feito com e-mail e senha cadastrados diretamente no Supabase.

Nenhuma credencial ou chave sensível é mantida neste README.

## Hospedagem

Site estático servido via GitHub Pages, diretamente a partir da branch `main` (pasta raiz), sem etapa de build.
