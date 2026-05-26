# AGENTS.md

## Arquitetura

Site estático de página única (`index.html`). Todo o HTML, CSS e JavaScript estão em um único arquivo.

## Estrutura

```
/
├── index.html       # Landing page completa (HTML + CSS + JS inline)
├── netlify.toml     # Configuração do Netlify — publish dir = "."
├── README.md
└── AGENTS.md
```

## Decisões relevantes

- **Single-file**: toda a página foi criada como arquivo HTML único com estilos e scripts inline — não há build step nem assets externos além de Google Fonts.
- **Checkout externo**: os botões de CTA apontam para `pay.hotmart.com` — não há lógica de pagamento no site.
- **Countdown**: calcula automaticamente o tempo até 12/06/2026 (Dia dos Namorados BR) via JavaScript no cliente.
