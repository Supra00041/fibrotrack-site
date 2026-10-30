# FibroTrack — Site institucional

Página de apresentação do **FibroTrack**, software de rastreabilidade da
desinfeção de fibroscópios. Publicada em **https://fibrotrack.pt**
(www.fibrotrack.pt redireciona para lá; o endereço do Netlify é
https://fibrotrack.netlify.app).

É um site **estático de um único ficheiro**, o `index.html`, com as imagens e as
fontes embutidas. Não precisa de build nem de dependências.

## Conteúdo

- **Hero** com um selo pequeno "✓ Piloto formal de 3 meses aprovado" e, logo a
  seguir, a faixa **"Apresentado em"** com o logótipo do IACS 2026 (recortado do
  modelo oficial do congresso) e "8.º Congresso Internacional · Outubro 2026".
  Dizer sempre "Apresentado em", nunca "parceiro" nem "apoiado por". Não se
  nomeia nenhuma instituição.
- Secção do problema, **Como funciona** (oito pontos, do cartão ao
  relatório do dia em PDF), **Rastreabilidade em segundos** (pesquisa por doente
  e por lote), demonstração, conformidade e auditoria, contacto e rodapé.
- **Capturas de ecrã** do software com **dados fictícios** (números de série,
  operadores, doentes e lotes inventados). Nunca usar capturas com dados reais.
- **Botão "Experimentar a demonstração no navegador"**, que abre
  https://fibrotrack-demo.netlify.app.
- **Contactos:** `fibrotrack.contacto@gmail.com` · **915 024 038**.
- **Formulário de contacto** ligado ao **Netlify Forms** (nome: `contacto`),
  com honeypot anti-spam (`bot-field`, escondido) e confirmação na própria
  página, também escondida até ao envio.

## Regras do texto

- Dizer sempre "software", nunca "app" ou "aplicação".
- Dizer "fibroscópios", nunca "endoscópios".
- Português de Portugal.
- Só afirmar o que o software faz e se pode mostrar. Não inventar números nem
  resultados.

## Como foi gerado

O `index.html` foi compilado a partir de um design exportado de um editor. O
conteúdo foi passado a HTML estático e os restos do editor foram removidos.
Para editar, altera-se o `index.html` diretamente.

## Publicação (Netlify via GitHub)

O projeto `fibrotrack` no Netlify está ligado a este repositório e publica
**automaticamente a cada push para `main`**. Um push é uma publicação.

- Publish directory: `.` (raiz), ver `netlify.toml`.
- Sem build command (site estático).
- O formulário aparece em **Netlify → Forms** depois da primeira publicação.

Para receber os pedidos por email: **Netlify → Forms → Settings → Form
notifications → Add notification → Email**.
