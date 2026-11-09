# Tradumix: catálogo de traduções

Catálogo público das traduções que o app [Tradumix](https://github.com/LamarcKz/Tradumix) mostra.
O app baixa o `indice-v2.json` deste repositório ao abrir e, na hora de traduzir, o patch da tradução
escolhida.

Este repositório só tem texto e os patches das traduções (`.xdelta`, nas releases). Nenhum jogo,
imagem ou vídeo é guardado aqui. Cada pessoa aplica o patch na própria ISO.

## Estrutura

| Caminho | O que é |
|---|---|
| `indice-v2.json` | Lista de traduções publicadas (formato 2, com a plataforma), descrita em `docs/catalogo.md` do app. |
| `indice.json` | A mesma lista no formato 1, lida pelas versões do app até a 0.2. |
| Releases | Um asset `.xdelta` por versão de tradução, com a tag `<id>-v<versão>`. |

## Capas e trailers

O catálogo guarda só referências:

- **Capa:** o app busca pelo serial do jogo no acervo público
  [xlenore/ps2-covers](https://github.com/xlenore/ps2-covers), o mesmo que o PCSX2 usa no
  Cover Downloader.
- **Trailer:** a ficha guarda o id do vídeo no YouTube (`midia.trailer_youtube`), e o app o mostra
  no player do próprio YouTube.

## Regras do catálogo

- Toda tradução preserva o hash do RetroAchievements: aplicada na ISO original, a ISO traduzida
  continua reconhecida pelas conquistas.
- Traduções de outras pessoas só entram com a permissão do autor, registrada na ficha, e com os
  créditos.
- O `sha256` e o `tamanho` de cada arquivo na ficha são conferidos pelo app em todo download.

## Licença

Cada tradução pertence aos seus tradutores, citados na ficha. Capas e trailers pertencem aos
respectivos detentores e não são hospedados neste repositório.
