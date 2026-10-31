# Meu Financeiro

App pessoal de finanças (casa + motorista de aplicativo). Um único arquivo `index.html`, sem build.

- Dados salvos no navegador e sincronizados com o Supabase (projeto "Meu Financeiro", tabela `app_state`, com RLS: cada usuário só lê e grava a própria linha).
- A chave que aparece no código é a chave **publicável** do Supabase, feita para ficar no navegador. Nunca coloque aqui a chave `service_role` / secreta.
- Os dados financeiros **não** ficam neste repositório; ficam só na sua conta.

## Publicar
Settings → Pages → Source: "Deploy from a branch" → Branch `main`, pasta `/ (root)`.
