<div align="center">

<img src="./public/logo.svg" width="80" height="80" alt="VEO Image Converter" />

# VEO Image Converter

**Conversão de imagens privada, rápida e 100% no navegador.**

<br/>

[![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev)
[![Vite](https://img.shields.io/badge/Vite-6-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org)
[![License](https://img.shields.io/badge/License-MIT-8B7CF6?style=for-the-badge)](./LICENSE)

<br/>

[![Live Demo](https://img.shields.io/badge/🌐_Abrir_Conversor-0A0A0A?style=for-the-badge)](https://veo-convertor.veo14269.workers.dev/)

</div>

---

## Sobre

O **VEO Image Converter** é uma aplicação web gratuita que converte e redimensiona imagens **sem enviar nada para nenhum servidor**.  
Tudo acontece localmente no seu navegador — privado, rápido e seguro.

Arraste um arquivo ou um lote inteiro, escolha o formato de saída e baixe o resultado.

---

## Funcionalidades

- Conversão **100% local** (Canvas + APIs nativas do navegador)
- Suporte a **lote** (vários arquivos de uma vez)
- Pré-visualização do original e do resultado
- **PNG** com transparência preservada
- **JPG / JPEG** com qualidade ajustável e fundo configurável
- Redimensionamento opcional (mantém proporção ou tamanho livre)
- Download individual ou **ZIP** completo
- Histórico da sessão atual
- Sanitização de SVG (remove referências externas)
- Interface responsiva em português brasileiro

---

## Formatos suportados

| Entrada | Saída |
|---------|-------|
| SVG, PNG, JPG, JPEG, WebP, GIF, BMP, AVIF | PNG, JPG, JPEG |

> GIFs animados são convertidos como um único quadro estático.

**Limites atuais**  
- 50 MB por arquivo  
- Até 50 arquivos por lote  
- 150 MB de entrada total  
- 16.384 px por lado / 40 megapixels  
- Resultados da sessão limitados a 200 MB

---

## Tecnologias

<div align="center">

[![Skills](https://skillicons.dev/icons?i=react,vite,ts,html,css,js,vscode,github&perline=8)](https://skillicons.dev)

</div>

Também utiliza: **Canvas API**, **JSZip** e sanitização de SVG.

---

## Como usar

1. Acesse o site: [veo-convertor.veo14269.workers.dev](https://veo-convertor.veo14269.workers.dev/)
2. Arraste as imagens ou clique em **Selecionar imagens**
3. Escolha o formato de saída (PNG / JPG / JPEG)
4. (Opcional) Defina largura e altura
5. Clique em **Converter imagens**
6. Baixe individualmente ou use **Baixar tudo (.ZIP)**

---

## Instalação local

Requisitos: **Node.js 20+** e npm.

```bash
git clone https://github.com/veo14269-jpg/veo-converdor.git
cd veo-converdor
npm ci
npm run dev
```

Abra o endereço que o Vite mostrar no terminal.

Para build de produção:

```bash
npm run build
npm run preview
```

---

## Estrutura do projeto

```text
public/               → Logo e favicon
src/components/       → Interface (header, upload, configs, preview)
src/services/         → Validação e conversão de imagens
src/styles/           → Estilos globais e responsivos
src/utils/            → Formatos e downloads
.github/workflows/    → Deploy no GitHub Pages
```

---

## Privacidade

- Nenhum arquivo sai do seu dispositivo
- Sem backend, sem contas, sem tracking
- Sem API keys e sem uploads
- SVGs são sanitizados antes do processamento

---

## Licença

Distribuído sob a licença **MIT**.  
Veja o arquivo [LICENSE](./LICENSE) para mais detalhes.

---

<div align="center">

Feito com ❤️ por [veo14269-jpg](https://github.com/veo14269-jpg)

</div>
