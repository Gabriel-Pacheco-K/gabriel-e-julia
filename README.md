# Gabriel & Julia — Nosso diário

Um álbum/diário digital em uma página só (`index.html`), sem dependências.

## Páginas

1. **Capa** — ex libris "Este diário pertence a Julia" com selo de cera
2. **Juntos há…** — torre com relógio e contador ao vivo (anos, meses, dias, horas, min, seg)
3. **Uma carta pra você** — envelope que abre e a carta se escreve sozinha
4. **O céu daquela noite** — a fase da lua calculada pra data em que vocês começaram
5. **Cabine de fotos** — duas tirinhas; o coração dourado "tira" novas fotos e o botão vermelho troca o filtro
6. **Dicionário do amor** — livro aberto com lupa que acompanha o dedo
7. **A nossa jornada** — 6 polaroids no varal de luzinhas (toque pra ampliar)
8. **Por que eu te amo** — pote dos motivos (toque ou chacoalhe o celular)
9. **O nosso retrato** — quebra-cabeça da foto de vocês no cavalete
10. **Continua…** — contracapa com o botão "aperte se você me ama"

Navegação: setas, arrastar para os lados ou teclado (← →). O ícone de som liga uma caixinha de música.

## Como personalizar

Tudo fica no bloco `CONFIG`, no topo do `index.html`:

- `inicio`: data e hora em que vocês começaram (alimenta o contador, a lua, a capa e o dicionário)
- `cidadeEle`, `cidadeEla`, `carta`, `motivos`, `momentos`, `dicionarioExemplo`
- `musica`: coloque um `musica.mp3` na pasta e escreva `"musica.mp3"` para tocar a música de vocês

## Fotos

As fotos ficam em `fotos/` (`01.jpg` … `15.jpg`) e são listadas em `CONFIG.fotos`, cada uma com um `foco` (onde ficam os rostos, para o recorte não cortar ninguém). Se faltar alguma, aparece um coração no lugar.
Os índices em `CONFIG` (`fotoLua`, `fotoRetrato`, `cabine`, `dicionario`, `momentos[].foto`) escolhem qual foto vai em cada lugar (0 = `01.jpg`).

## Publicar no GitHub Pages

1. Crie um repositório e suba `index.html` e a pasta `fotos/`
2. Em **Settings → Pages**, escolha a branch `main` e a pasta `/ (root)`
3. O link fica `https://<seu-usuario>.github.io/<nome-do-repo>/`
