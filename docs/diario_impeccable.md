# Diário Impeccable — Portfólio Carlos Alexandre (v2)

> Registro contínuo das intervenções da metodologia Impeccable sobre o portfólio.
> Uma linha por intervenção. Nada sai daqui sem virar aprendizado para a próxima passada.

- **Projeto:** Portfólio Profissional — Carlos Alexandre
- **Mundo visual comprometido:** Brutalismo + Dark Academia / colagem digital (branco × preto, destaque cobalto `#0000FF`)
- **Base técnica:** Bootstrap 5 · `index.html` · `css/style.css` · `js/script.js`
- **Início da v2:** 2026-09-21

## Como registrar

Copie a linha-modelo abaixo para cada nova intervenção:

```md
| AAAA-MM-DD | comando | seção/arquivo | o que mudou e por quê | status |
```

**Comandos válidos:** `init` · `document` · `shape` · `critique` · `audit` · `polish` · `bolder` · `quieter` · `adapt` · `animate` · `live`
**Status válidos:** `Feito` · `Em revisão` · `Revertido`

## Intervenções

| Data | Comando | Seção / Arquivo | O que mudou e por quê | Status |
| ---- | ------- | --------------- | --------------------- | ------ |
| 2026-09-21 | init | raiz → `css/` · `js/` · `docs/` | Estrutura v2 isolada: `style.css` → `css/style.css`, `script.js` → `js/script.js`; caminhos atualizados no `index.html`. Prepara o terreno para as melhorias sem quebrar nada. | Feito |
| 2026-09-21 | document | `docs/diario_impeccable.md` | Criado este diário com cabeçalho e tabela de registro para as intervenções da v2. | Feito |
| 2026-09-21 | shape | `css/style.css` → `#habilidades` · `#projetos` | Trocado o grid rígido por offsets propositais: colunas com `margin-top` escalonado, sobreposição por `margin-left` negativo e `z-index` em camadas, rotações individuais via variáveis `--tilt`/`--drop`. Tudo contido em `overflow: clip` e zerado abaixo de `lg` para preservar o empilhamento responsivo do Bootstrap. | Feito |
| 2026-09-21 | polish | `css/style.css` (lote pós-detector) | Detector: 43 achados, corrigidos os defeitos reais em 1 lote — captions 0.68→0.72rem (piso 11px), tracking de parágrafo 0.08→0.03em, tinta `--cobalto-no-preto` p/ ícones/níveis sobre fundo preto (contraste AA), `prefers-reduced-motion` pausa ticker/transições. Mantidos por decisão do mundo cometido: bordas 3px, kickers numerados, ticker, sombras duras, Inter de apoio. | Feito |
| 2026-09-21 | critique | `index.html` → `#sobre` `.break-out-text` | Lead de 4 frases (~45 palavras) encurtado para 2 (~22): mantém C/Java/PHP + ETEC/IFSP + objetivo, corta a redundância. Leitura escaneável, ritmo brutalista. Formação mantida — descrições dos cards já são telegráficas. | Feito |
| 2026-09-21 | audit | `index.html` → `#projetos` imgs + ícones `bi-*` | Imagens verificadas: 3 placeholders P&B já corretos com `alt=""` + `aria-hidden` (decorativas, WCAG ok) e `avatar-selo` com `role="img"` + `aria-label`. Corrigido o gap real: 14 ícones Bootstrap sem `aria-hidden="true"` — todos decorativos (sempre acompanhados de texto), agora silenciados p/ leitores de tela. | Feito |
| 2026-09-21 | remove | `index.html` + `css/style.css` → `.deco-triangle-2` | Removido o triângulo sobre `#habilidades`: 4ª camada decorativa (star + graph + TECHNÉ gigante) cruzando os cards sem acrescentar informação. Regra CSS e referência no media-query limpas junto. | Feito |
| 2026-09-21 | flatten | `index.html` → containers das 5 seções + `#formacao` row + `#projetos` col | Removidos 7 `position-relative` redundantes: `.content-layer` já é `position: relative`, então a classe do Bootstrap só duplicava. Mantidos os 2 com propósito (container da navbar, coluna que ancora `.avatar-selo` absoluto). HTML mais limpo, layout idêntico. | Feito |
| 2026-09-21 | align | `css/style.css` → `#habilidades` · `#formacao` | Cascata mantida por fora, régua por dentro: corpos dos cards viram coluna flexível com descrição `flex:1` e linha `.nivel` presa à base (baselines iguais nos 3 cards); na Formação a linha do curso ganhou `min-height: 3em` para os badges Concluído/Cursando sentarem na mesma régua. Desalinho deliberado, nunca acidental. | Feito |
| 2026-09-21 | scale | `css/style.css` → tipografia | Títulos de seção `clamp(2.2rem,…,3.6rem)` → `clamp(2.6rem,6vw,4.2rem)` (claros até 4rem); apoio `.texto-apoio` com corpo `0.95rem`. Nota honesta: Inter 300 já é o peso mais leve carregado, então o contraste foi construído no tamanho, não no peso. | Feito |
| 2026-09-21 | refine | `css/style.css` → bordas e sombras | `--borda` 2px → `3px solid` preto em todo o sistema (cards, botões, badges, toggler, selo); sombras duras sem blur 7px → 8px (hover 12px); cobalto `#0000FF` preservado como única cor de sombra/linha. Removida regra `.card-tcc` redundante. | Feito |
| 2026-09-21 | minify | `css/style.min.css` (12,2 KB) · `js/script.min.js` (763 B) | Minificação com tokenizer que preserva literais de string (1ª tentativa ingênua corrompia espaços/acentos dentro de `alert`/`console` — refeita com split por `"..."` e I/O UTF-8 explícito; strings verificadas byte a byte). `index.html` agora referencia os `.min` em produção; fontes seguem no repo p/ desenvolvimento. | Feito |
| 2026-09-21 | validate | `index.html` · `css/style*.css` · `js/script*.js` | Sem erros: tags HTML balanceadas (22 tipos conferidos), chaves CSS 152/152 nos dois arquivos, comentários 25/25 → 0/0 no min, `node --check` passa nos dois JS. Validação pronta p/ W3C. | Feito |
| 2026-09-21 | export | raiz do repo → GitHub Pages | Estrutura final: `index.html` na raiz, `css/` + `js/` (fontes e min), `docs/` isolada; nenhum caminho local (`C:\`, `file://`); só relativos + CDN/placeholders externos. Pronto p/ deploy: basta push e ativar Pages no branch. | Feito |
