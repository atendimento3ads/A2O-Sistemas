# A²O Sistemas — Wireframe

Wireframe estrutural navegável do site da A²O Sistemas (esqueleto em preto e branco, sem identidade visual final).

- `index.html` — wireframe completo (arquivo único, navegação interna por JavaScript, sem dependências externas além do Google Fonts).
- `docs/` — material de origem (Definição e Estratégia).

## Estrutura

```
.
├── index.html        # site (página servida pela hospedagem)
├── .cpanel.yml       # tarefas de deploy do cPanel Git Version Control
├── .gitignore
├── README.md
└── docs/             # documentos de referência (não vão para o ar)
```

## Deploy via cPanel (Git Version Control)

1. No cPanel, abra **Git™ Version Control** e crie/clique no repositório.
2. Em **Pull or Deploy → Deploy HEAD Commit**, o cPanel lê o arquivo `.cpanel.yml`.
3. Antes do primeiro deploy, edite o `.cpanel.yml` e troque `USUARIO` pelo usuário real da conta
   (o caminho costuma ser `/home/SEU_USUARIO/public_html`).
4. Faça `git push` para o repositório do cPanel e clique em **Deploy HEAD Commit**.

O deploy copia o `index.html` para o `public_html`, publicando o site.

## Rodar localmente

Basta abrir o `index.html` no navegador (funciona offline).
