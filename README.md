# Notícias do Mundo — versão inicial

Aplicação web instalável (PWA) para Android, com fontes de Moçambique, Angola, Brasil e Estados Unidos.

## Funcionalidades
- Diretório de fontes e abertura dos sites oficiais.
- Filtros por país, perfil editorial e tipo de publicação.
- Favoritos guardados no navegador/dispositivo.
- Pesquisa de notícias e comparação por tema usando pesquisas externas do Google News.
- Cache básico da interface para facilitar reabertura.
- Manifesto e ícones para instalação como aplicação web.

## Importante
Esta é uma primeira versão funcional do diretório e da comparação por pesquisas externas. Não agrega ainda feeds RSS diretamente dentro da página. Para essa funcionalidade, é necessário validar os feeds e escolher uma forma de leitura que respeite CORS, direitos de autor e termos de cada fonte. As orientações editoriais são estimativas e devem ser verificadas; não indicam qualidade nem veracidade.

## Publicar no GitHub Pages pelo telemóvel
1. Crie um repositório novo chamado `noticias-do-mundo` (recomendado, para não alterar `biblioteca-reformada`).
2. Extraia este ZIP.
3. No repositório, escolha **Add file → Upload files** e carregue `index.html`, `manifest.json`, `service-worker.js` e a pasta `icons`.
4. Faça **Commit changes**.
5. Em **Settings → Pages**, selecione a publicação a partir da branch principal e da pasta `/ (root)`.
6. Aguarde a publicação e abra a URL `https://SEU-USUARIO.github.io/noticias-do-mundo/`.
7. No Chrome Android, menu ⋮ → **Adicionar ao ecrã inicial** ou **Instalar app**, se a opção aparecer.

## Notas
- O GitHub Pages usa HTTPS, requisito para service workers/PWA.
- Não coloque chaves privadas ou credenciais no HTML.
- Verifique os endereços das fontes antes de divulgar publicamente.
