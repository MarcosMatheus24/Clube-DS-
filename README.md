# Clube D/S — React

```
npm install
cp .env.example .env     # coloque o link do WhatsApp (e, se quiser, os dominios de e-mail)
npm run dev              # http://localhost:5173
```
Requer Node 18 ou superior. Para publicar (Vercel), adicione as variaveis `VITE_*` do `.env` nas configuracoes do projeto; o `vercel.json` ja trata as rotas.

Fluxo: botao "Quero participar" -> pagina `/participar` -> formulario -> mensagem de sucesso + secao da comunidade com o botao do WhatsApp.
Os dados do formulario nao sao armazenados.

Professores: edite `src/dados.js` (nome, cargo, areas e foto em `public/professores/`). Cursos do formulario tambem ficam la.

Equipe e hackathon: em `src/dados.js`, troque os nomes do presidente e do vice em `LIDERES` e, quando quiser, liste os projetos do Power Tech Hackathon em `PROJETOS_HACKATHON` (a grade so aparece quando a lista tem itens). As fotos ficam em `public/equipe/`.
