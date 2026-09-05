# ChurchView

Ferramenta web para exibir versículos bíblicos em telão/segunda tela durante cultos, com controle em uma janela e projeção em outra.

Arquivo único: `biblia.html`. Sem build, sem dependências, sem backend.

## Uso

1. Abra `biblia.html` no navegador (controlador).
2. Pesquise um versículo (ex: `João 3:16`) ou um intervalo (ex: `Lucas 11:5-13`).
3. Clique nos resultados para montar uma cadeia de versículos.
4. Clique em **Abrir apresentação** para abrir a segunda janela (arraste para o projetor e dê dois cliques para tela cheia).
5. Use **Enviar para apresentação**, os botões Anterior/Próximo ou as setas do teclado (`←` `→`) para navegar.

## Funcionalidades

- Busca por referência única ou intervalo de versículos.
- Cadeia de versículos: adicionar, reordenar, remover, navegar (Anterior/Próximo, com contador `X / Y`).
- Sugestão de imagens de fundo por tema (via LoremFlickr).
- Fonte do texto ajustada automaticamente ao tamanho do container, na apresentação e no preview.
- Sincronização entre a janela de controle e a de apresentação via `localStorage`.

## Fonte dos versículos

Texto da versão pública **Almeida Livre** (domínio público), servido sem chave via
[`midvash/bible-data`](https://github.com/midvash/bible-data) no GitHub. Não requer conta, login ou variável de ambiente — funciona direto em hospedagem estática (GitHub Pages incluso).

## Limitações atuais

- Sincronização entre janelas via `localStorage` é mais confiável servindo o arquivo por `http://` do que abrindo direto como `file://`.
- Imagens de fundo dependem de disponibilidade do LoremFlickr; sem internet, a busca de imagens falha.
