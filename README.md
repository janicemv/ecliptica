# Eclíptica

Movimento retrógrado aparente dos planetas.

Abra [`index.html`](index.html) no navegador: ele traz uma barra lateral de navegação com acesso às quatro visualizações do projeto, exibidas em um painel à direita.

## Páginas

- [`Ecliptica-animado.html`](Ecliptica-animado.html) — animação das órbitas do sistema solar ao redor do Sol e da faixa do zodíaco.
- [`ecliptica_movimento_retrogrado.html`](ecliptica_movimento_retrogrado.html) — simulação interativa (Terra × planeta) que ilustra por que um planeta parece andar para trás no céu.
- [`duracao_frequencia_retrogrados.html`](duracao_frequencia_retrogrados.html) — comparação da duração típica e do intervalo entre os retrógrados de cada planeta.
- [`timeline.html`](timeline.html) — linha do tempo da história do culto às estrelas, da Mesopotâmia às reinterpretações contemporâneas.

Essas páginas também podem ser abertas individualmente, fora do `index.html`.

## Editando a linha do tempo

O conteúdo de `timeline.html` vem de [`timeline.md`](timeline.md). Para atualizar, edite o `.md` seguindo o formato:

- `# Título` na primeira linha define o título da página.
- `# Nome da era` (sem `##` antes) cria um divisor de era.
- `## data` seguido de `# título` cria um evento.
- `- item` cria um marcador; `    - item` (indentado) cria um sub-item.

No GitHub Pages a página busca o `.md` automaticamente ao carregar — basta commitar e dar push. Para testar localmente, é preciso servir os arquivos por `http://` (abrir o `.html` direto como arquivo bloqueia essa busca no navegador):

```
python3 -m http.server 8000
```

e acessar `http://localhost:8000/timeline.html`.

## Estrutura

- `img/` — recursos visuais (logo).
- `timeline.md` — dados da linha do tempo (fonte de conteúdo do `timeline.html`).
