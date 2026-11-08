<div align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=html,css,js,ts,json,vscode,github,android,windows,linux,apple&perline=6" alt="HTML, CSS, JavaScript, TypeScript, JSON, VS Code, GitHub, Android, Windows, Linux e Mac" />
  </a>
  <h1>VEO Image Converter</h1>
  <p>Conversão de imagens privada, prática e diretamente no seu navegador.</p>
  <p>
    <img alt="React" src="https://img.shields.io/badge/React-18-149ECA?logo=react&logoColor=white" />
    <img alt="Vite" src="https://img.shields.io/badge/Vite-6-646CFF?logo=vite&logoColor=white" />
    <img alt="Privacidade local" src="https://img.shields.io/badge/Processamento-100%25%20local-35A878" />
    <img alt="Licença MIT" src="https://img.shields.io/badge/Licen%C3%A7a-MIT-8B7CF6" />
    <img alt="GitHub Copilot" src="https://img.shields.io/badge/GitHub%20Copilot-000000?logo=githubcopilot&logoColor=white" />
  </p>
</div>

## Apresentação

O **VEO Image Converter** é uma aplicação web gratuita para converter e redimensionar imagens sem enviá-las a um servidor. Adicione um arquivo ou um lote, escolha PNG, JPG ou JPEG e baixe cada resultado ou um arquivo ZIP.

## Funcionalidades

- Conversão local com Canvas e APIs nativas do navegador.
- Conversão em lote sequencial, sem interromper os demais arquivos quando um falha.
- Pré-visualização do original e do resultado.
- PNG com transparência preservada; JPG/JPEG com qualidade ajustável e cor de fundo configurável.
- Redimensionamento com dimensões personalizadas e proporção opcional.
- Renomeação e download individual ou em ZIP.
- Histórico mantido somente durante a sessão atual.
- Sanitização de SVG, sem carregar referências externas automaticamente.
- Limites para quantidade, tamanho, dimensões e memória dos arquivos.
- Interface responsiva em português brasileiro.

## Formatos

**Entrada:** SVG, PNG, JPG, JPEG, WebP, GIF, BMP e AVIF. A decodificação depende do navegador e do dispositivo. GIFs animados são convertidos como um único quadro estático.

**Saída:** PNG, JPG e JPEG. JPG e JPEG usam a codificação JPEG do navegador; a diferença é apenas a extensão do arquivo.

Limites atuais: 50 MB por arquivo, 50 arquivos e 150 MB de arquivos de entrada por lote, 16.384 px por lado e 40 megapixels por imagem. Os resultados da sessão são limitados a 200 MB. Esses limites protegem a memória do navegador.

## Tecnologias

<p align="center">
  <a href="https://skillicons.dev"><img src="https://skillicons.dev/icons?i=html,css,js,ts,json,vscode,github,android,windows,linux,apple&perline=6" alt="HTML, CSS, JavaScript, TypeScript, JSON, VS Code, GitHub, Android, Windows, Linux e Mac" /></a>
</p>
<p align="center">
  <a href="https://github.com/features/copilot"><img src="https://img.shields.io/badge/GitHub%20Copilot-000000?style=for-the-badge&logo=githubcopilot&logoColor=white" alt="GitHub Copilot" /></a>
</p>

O projeto também utiliza React, TSX, Vite, TypeScript, CSS, HTML5, Canvas API e JSZip.

## Instalação e execução

Requisitos: Node.js 20 ou superior e npm.

```bash
git clone https://github.com/SEU_USUARIO/veo-image-converter.git
cd veo-image-converter
npm ci
npm run dev
```

Abra o endereço local mostrado pelo Vite. Para gerar e testar a versão de produção:

```bash
npm test
npm run build
npm run preview
```

## Como converter

1. Arraste imagens para a área de envio ou selecione arquivos no dispositivo.
2. Escolha PNG, JPG ou JPEG. Para JPEG, ajuste a qualidade e o fundo usado nas áreas transparentes.
3. Opcionalmente, abra **Redimensionar imagem** para informar largura e altura.
4. Selecione **Converter imagens**. Os arquivos são processados localmente, um por vez.
5. Baixe cada imagem individualmente ou escolha **Baixar tudo (.ZIP)**.

## Estrutura

```text
public/                  Identidade visual e favicon
src/components/          Cabeçalho, envio, configurações, prévias e histórico
src/services/            Validação, leitura e conversão de imagens
src/styles/              Estilos globais e componentes responsivos
src/utils/               Formatos e downloads
src/test/                Configuração dos testes
.github/workflows/       Build, testes e publicação no GitHub Pages
```

## Privacidade

Os arquivos permanecem no dispositivo e são processados pelo navegador. O projeto não possui backend, contas, rastreamento, API keys ou uploads. Recursos referenciados externamente em SVGs são removidos antes do processamento. As fontes da interface podem ser carregadas do Google Fonts; a conversão de imagens continua inteiramente local.

## Publicação no GitHub Pages

1. Envie o projeto para um repositório público com a branch principal chamada `main`.
2. Em **Settings → Pages → Build and deployment**, selecione **GitHub Actions** como fonte.
3. Envie um commit para `main` ou execute manualmente o workflow **Publicar no GitHub Pages** na aba **Actions**.
4. Aguarde os jobs de teste, build e deploy. O endereço publicado aparece nas configurações de Pages.

O Vite utiliza caminhos relativos, portanto a aplicação funciona tanto em domínios próprios quanto em repositórios de projeto no Pages.

## Licença

Distribuído sob a licença MIT. Consulte [LICENSE](./LICENSE).
