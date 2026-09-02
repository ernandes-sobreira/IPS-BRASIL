
# IPS Brasil 2026 — v11

Correção específica da busca global de indicadores.

## Correção

Na v10, a seleção pelo teclado (Enter) funcionava, mas em alguns navegadores o clique do mouse nos resultados da busca não disparava a seleção.

Na v11:

- cada resultado da busca é um botão HTML nativo;
- a seleção ocorre em `pointerdown`, antes de eventos de perda de foco (`blur`) e do `click` tradicional;
- funciona com mouse, touchpad e toque;
- o identificador passado pelo evento é apenas um índice numérico, evitando problemas com aspas e caracteres especiais nos nomes dos indicadores;
- Enter e setas do teclado continuam funcionando.

A interação por clique foi testada em navegador automatizado antes da entrega.

## Integridade dos dados

- `conhece_brasil_v1.json`: IDÊNTICO
  - SHA-256: `6a6a6e190a2d919ac068f412c56a3486183130249f525ed5d1ea18ec6849f517`
- `municipios_topo.json`: IDÊNTICO
  - SHA-256: `6582b9afd36021473f7f138df530d5b0297a612dd1d4428e561270f01cb26c02`
- `municipios_geo.geojson`: IDÊNTICO
  - SHA-256: `c4892567054ddd69b34d182efb1a4425234622aa47eb34a3774daef971c2a892`
