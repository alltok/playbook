# Alltok Playbook

Como a Alltok descobre, valida, constrói e decide sobre seus produtos.

Página única (one-page), em HTML/CSS/JS puro, sem build e sem dependências além da fonte IBM Plex Sans (Google Fonts).

**Publicado em:** https://alltok.github.io/playbook/

## Estrutura

| Arquivo | Função |
| --- | --- |
| `index.html` | Página completa (conteúdo, estilos e scripts) |
| `.nojekyll` | Impede o processamento Jekyll do GitHub Pages |
| `.github/workflows/pages.yml` | Deploy automático a cada push na `main` |
| `LICENSE` | CC0 1.0 |

## Publicar

1. Envie os arquivos para a branch `main` do repositório `alltok/playbook`.
2. Em **Settings → Pages → Build and deployment → Source**, escolha **GitHub Actions**.
3. A cada push na `main` o site é atualizado em `https://alltok.github.io/playbook/`.

> Alternativa sem Actions: em **Source**, escolha **Deploy from a branch**, branch `main`, pasta `/ (root)`. Nesse caso, apague a pasta `.github`.

## Testar localmente

```bash
python3 -m http.server 8000
# abra http://localhost:8000
```

O Product Ledger e o tema claro/escuro são salvos no `localStorage` do navegador.
