# FibroTrack — Site institucional

Landing page do **FibroTrack** (rastreabilidade da desinfeção de endoscópios),
publicada em **https://fibrotrack.netlify.app**.

É um site **estático de um único ficheiro** — `index.html` — com **todas as
imagens, fontes e o traçado do vídeo embutidos**. Não precisa de build nem de
dependências. O vídeo é incorporado do YouTube (via `youtube-nocookie`).

## Conteúdo

- **Hero**, secção do problema, "três passos" com fotografias, vídeo de 90s,
  bloco de demo, conformidade/auditoria, credibilidade, contacto e rodapé.
- **Botão "Experimentar a demo no browser"** → https://fibrotrack-demo.netlify.app
- **Contactos:** `geral@fibrotrack.pt` · **915 024 038**
- **Formulário de contacto** ligado ao **Netlify Forms** (nome: `contacto`),
  com honeypot anti-spam (`bot-field`) e confirmação inline sem sair da página.

## Como foi gerado

O `index.html` foi compilado a partir do design exportado (formato de editor):
o conteúdo foi renderizado para HTML estático, os `<image-slot>` convertidos em
`<img>` reais, e todos os restos do editor removidos. Para editar, altera o
`index.html` diretamente.

## Publicação (Netlify via GitHub)

O projeto `fibrotrack` no Netlify está ligado a este repositório e faz
**deploy automático** a cada push para `main`:

- Publish directory: `.` (raiz) — ver `netlify.toml`
- Sem build command (site estático)
- Formulário: aparece em **Netlify → Forms** após o primeiro deploy

Para receber os pedidos por email: **Netlify → Forms → Settings → Form
notifications → Add notification → Email**.
