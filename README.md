# Sabionet Anim

Biblioteca com as ilustrações animadas da Sabionet para o site (Webflow) e landing pages.

## Uso no Webflow
1. **Site settings › Custom code › Footer code** (uma vez):
   ```html
   <script src="https://SEU-PROJETO.vercel.app/v/1.0.2/sabionet-anim.js" defer></script>
   ```
2. Em cada página, um elemento **Embed** com a peça:
   ```html
   <sbn-anim piece="CUR-01" theme="light" lang="pt"></sbn-anim>
   ```

Atributos: `piece` · `theme` (light | dark | auto) · `lang` (pt; es em breve) · `ratio` (opcional, ex.: 4/5) · `background="none"` (opcional). Cantos: `style="--sbn-radius:0"`.

## Versões
- `/v/1.0.2/sabionet-anim.js` — versão fixa (recomendada no site; nunca muda).
- `/sabionet-anim.js` — sempre a última versão.

Para publicar uma versão nova: adicione a pasta `v/1.1.0/` com o arquivo novo, atualize o `sabionet-anim.js` da raiz, faça commit. Depois troque o número da versão no Footer code do Webflow quando quiser adotar.

## Teste
Abra a URL do projeto na Vercel: a página inicial mostra todas as peças carregadas pela biblioteca.
