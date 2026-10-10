# Notícias do Mundo — pacote v2

Esta é uma aplicação web instalável (PWA) para Android, com diretório de fontes de notícias e ferramentas de pesquisa/comparação.

## Conteúdo do pacote
- `index.html`: interface e funcionalidades.
- `manifest.json`: configuração da aplicação instalável.
- `service-worker.js`: cache básico e suporte offline para a interface.
- `icons/`: ícones PNG de 192, 512 e 1024 px, além de favicon SVG.

## Publicação correta no GitHub Pages
1. Descarregue e extraia o ZIP.
2. Crie um repositório separado chamado `noticias-do-mundo`.
3. Dentro do repositório, carregue os ficheiros que estão **dentro** da pasta extraída: `index.html`, `manifest.json`, `service-worker.js` e a pasta `icons`. Não carregue apenas a pasta que contém tudo.
4. Faça commit.
5. Abra Settings → Pages → Build and deployment; escolha Deploy from a branch, branch `main` (ou a branch principal do repositório) e pasta `/(root)`.
6. Aguarde a publicação. Abra o endereço HTTPS indicado pelo GitHub Pages.
7. No Chrome Android, abra o site publicado, toque em ⋮ e escolha “Instalar app” ou “Adicionar ao ecrã inicial”.

## Se ainda não aparecer a opção de instalar
- Confirme que está a abrir o endereço publicado `https://...github.io/noticias-do-mundo/`, não um ficheiro local ou a pré-visualização do GitHub.
- Confirme que `manifest.json` e `service-worker.js` abrem no navegador sem erro.
- No Chrome, abra o site publicado, toque no ícone de definições do site e limpe os dados do site; depois recarregue.
- O menu pode dizer “Adicionar ao ecrã inicial” em vez de “Instalar app”. Isso cria um atalho, mesmo quando o Chrome não oferece instalação PWA completa.
- A instalação PWA exige HTTPS. O GitHub Pages fornece HTTPS quando o site está publicado corretamente.

## Limitações
A versão inclui diretório, filtros, favoritos e pesquisas externas. Não apresenta ainda todos os artigos automaticamente dentro da aplicação; isso requer feeds RSS/API compatíveis e validação das permissões de cada fonte. As etiquetas editoriais são aproximadas, não são uma avaliação da veracidade.
