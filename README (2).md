# Direito Certo

Protótipo funcional do app **Direito Certo** — Núcleo de Orientação Previdenciária Popular.

Aplicativo estático (HTML + CSS + JS puro, um único arquivo), sem servidor, sem build. Roda em qualquer navegador, inclusive celular.

## Estrutura

```
direito-certo/
└── index.html   ← o app inteiro (marcação, estilo e lógica)
```

## Rodar localmente

Basta abrir o `index.html` no navegador (duplo clique) ou, para simular melhor o comportamento de um site publicado:

```bash
python3 -m http.server 8000
# depois abra http://localhost:8000
```

## Publicar no GitHub Pages

1. Suba este arquivo para um repositório no GitHub, mantendo o nome `index.html` na raiz.
2. No repositório, vá em **Settings → Pages**.
3. Em **Build and deployment → Source**, escolha **Deploy from a branch**.
4. Em **Branch**, selecione `main` (ou `master`) e a pasta `/ (root)`. Salve.
5. Aguarde 1–2 minutos. O GitHub mostra o link no formato `https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/`.

Esse link já é público e pode ser mandado para qualquer pessoa testar no celular.

## O que ajustar antes de divulgar

- **Número de WhatsApp**: procure a constante `WHATSAPP_NUMBER` no início do `<script>` dentro do `index.html` e troque pelo número real (DDI+DDD+número, só dígitos, ex: `5547999999999`).
- **Conteúdo previdenciário**: cada categoria e checklist precisa de revisão técnica de alguém da área antes de ir ao ar, como aponta o briefing do projeto.
