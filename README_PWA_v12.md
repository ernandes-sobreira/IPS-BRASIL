# IPS Brasil 2026 — versão instalável (PWA v12)

Este pacote transforma o IPS Brasil em um **Progressive Web App (PWA)**. Depois de publicado em HTTPS (como no GitHub Pages), o usuário pode instalar o site no celular e abrir pelo ícone da tela inicial, com aparência de aplicativo.

## Arquivos que devem ficar juntos na raiz do GitHub Pages

- `index.html`
- `conhece_brasil_v1.json`
- `municipios_geo.geojson`
- `municipios_topo.json`
- `favicon.svg`
- `favicon-32.png`
- `favicon.ico`
- `manifest.webmanifest`
- `service-worker.js`
- `apple-touch-icon.png`
- `icon-192.png`
- `icon-512.png`
- `icon-maskable-512.png`

## O que foi adicionado no index

- referência ao `manifest.webmanifest`;
- suporte ao ícone de iPhone/iPad;
- registro do `service-worker.js`;
- botão **Instalar** no cabeçalho quando a instalação estiver disponível;
- instrução específica para iPhone/iPad.

## Como instalar no Android

1. Abra o IPS pelo Chrome.
2. Se aparecer o botão **Instalar** no topo do IPS, toque nele.
3. Confirme a instalação.
4. Se o botão não aparecer, abra o menu ⋮ do Chrome e escolha **Instalar app** ou **Adicionar à tela inicial**.

## Como instalar no iPhone/iPad

1. Abra o IPS no **Safari**.
2. Toque no botão **Compartilhar**.
3. Escolha **Adicionar à Tela de Início**.
4. Confirme em **Adicionar**.

## Observação sobre funcionamento offline

A estrutura do app e os ícones ficam em cache. Os arquivos de dados municipais são armazenados pelo navegador depois que forem carregados pela primeira vez. Recursos externos (como bibliotecas e mapas-base) ainda podem depender de internet.

## GitHub Pages

No repositório `ernandes-sobreira/IPS-BRASIL`, envie todos os arquivos acima para a branch `main`, na raiz do repositório. O GitHub Pages já serve o projeto por HTTPS, requisito para PWA.
