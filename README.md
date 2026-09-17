# evachat.intelliway.com.br

Site institucional do IntelliDesk (plataforma da Intelliway operada no Brasil,
região Oracle sa-saopaulo-1), servido por GitHub Pages em
`evachat.intelliway.com.br`. Mesma estrutura do
site do VipDesk — é dele que esta versão foi derivada.

## Publicar

1. Suba este diretório num repositório **público** (Pages gratuito exige público).
2. *Settings → Pages → Source*: `main` / raiz.
3. *Custom domain*: `evachat.intelliway.com.br` (o arquivo `CNAME` já está aqui).
4. No DNS (Cloudflare da intelliway.com.br), um registro **CNAME**:

   ```
   evachat  CNAME  monitchat.github.io
   ```

   Nuvem **cinza** (DNS only) até o GitHub emitir o certificado; depois pode
   voltar a proxiar se quiser.
5. Aguarde o certificado e marque **Enforce HTTPS**.

## Por que o conteúdo é o que é

Esta página também serve de *home page* na verificação do app no Google
(tela de consentimento OAuth). Por isso ela precisa, obrigatoriamente:

- identificar o produto **pelo nome** e descrever o que ele faz;
- ter uma seção sobre a **integração de agenda**, que é o que justifica os
  escopos `calendar.events` e `calendar.freebusy` pedidos ao usuário;
- linkar Política de Privacidade e Termos de Uso;
- identificar a empresa responsável.

Se for reescrever o texto, preserve esses quatro pontos — o revisor do Google
compara esta página com os escopos solicitados.

## O que muda em relação ao vipdesk.com.br

| Item | Valor |
|---|---|
| Marca | IntelliDesk (`Intelli` + `Desk` em negrito) |
| Cor | `#ac222a` (vermelho da Intelliway), apoio `#7d1720` e `#e0803a` |
| Empresa | Intelliway Tecnologia Ltda · CNPJ 21.337.573/0001-85 |
| Endereço | Rua Roberto da Silva, 20, Ed. Premium Office, Sala 309 — Mata da Praia, Vitória/ES, CEP 29066-091 |
| Contato | contato@intelliway.com.br · dpo@intelliway.com.br |
| Plataforma | https://app.evachat.intelliway.com.br |
| Foro (Termos) | comarca de Vitória/ES |

Os logos em `assets/` vieram do próprio front (`icon-512.png` e `icon-192.png`).
Se a Intelliway tiver uma versão horizontal com o nome escrito, troque
`assets/intellidesk-logo.png` — é ela que aparece no cabeçalho e no rodapé.
