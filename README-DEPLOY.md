# NEON PALMS — página de vendas (HTML estático)

## Antes de publicar (edite no index.html)
1. Procure `CHECKOUT_URL` (bloco de configuração no final do arquivo) e cole o link do checkout. Troque também os dois `href="CHECKOUT_URL_AQUI"` dos botões, se preferir.
2. `PIXEL_ID`: cole o ID do pixel do Meta. Deixe `SEU_PIXEL_ID` para manter desativado.
   Pixel e cookies exigem aviso e consentimento (LGPD): alinhe com o advogado antes de ativar.
3. `SEU_EMAIL@AQUI` no rodapé e o campo de CNPJ/CPF e razão social.
4. Links de Termos, Privacidade e Reembolso estão em `#`: crie as páginas com texto aprovado pelo advogado e troque os links.
5. Quando tiver um vídeo de amostra feito com material SEU, descomente o bloco `<video>` na seção "Monte a gosto" e salve o arquivo em `assets/amostra.mp4`. Não use trailer, trecho oficial de jogo nem vídeo de terceiros.
6. Confirme na página oficial da Anthropic os requisitos e planos do Claude Code antes de publicar.

## Publicar com GitHub + Vercel
1. Crie um repositório no GitHub e envie esta pasta (index.html, assets/, vercel.json).
2. No Vercel: Add New > Project > importe o repositório. Framework: "Other". Não precisa de build. Deploy.
3. (Opcional) Domínio próprio em Settings > Domains.
4. Teste no celular: botão de compra, link do checkout com UTM (`?utm_source=...`), pixel (extensão Meta Pixel Helper) e velocidade.

## Teste de UTM
Abra `https://seu-site.vercel.app/?utm_source=teste&utm_campaign=x` e clique em comprar: o checkout deve abrir com os mesmos parâmetros.

Conteúdo independente, não afiliado a nenhum estúdio de jogos nem à Anthropic.
