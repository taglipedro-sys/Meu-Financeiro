# Meu Financeiro

App pessoal de finanças (casa + motorista de aplicativo) em um único arquivo, `index.html`, sem etapa de build. Publicado pelo GitHub Pages a partir da branch `main`.

## Regras de trabalho

- **Sempre fazer o merge.** Depois de terminar e testar uma alteração, abrir o pull request para a `main` e fazer o merge em seguida, sem pedir confirmação. Pedido do dono do projeto.
- Antes do merge, testar a alteração no navegador e rodar os testes que já existem. Se algum teste falhar, corrigir antes; nunca fazer o merge com teste falhando.
- A `main` vai direto para o app publicado. Depois do merge, avisar que o site leva 1 a 2 minutos para atualizar.
- Nunca colocar dados financeiros no repositório (backups, exportações, arquivos `.json`/`.xls`/`.xlsx` com lançamentos). Eles ficam só na conta do usuário.
- Nunca colocar a chave `service_role` / secreta do Supabase no código. A chave que está lá é a publicável.

## Cuidados com os dados do usuário

- Importar ou sincronizar nunca pode apagar dados sem que o usuário veja antes o que será apagado.
- Qualquer mudança no formato dos dados precisa passar por `fix()` / `sane()`, para que backups antigos continuem abrindo.
