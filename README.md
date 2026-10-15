# ARKO IMPORTS

Site vitrine da ARKO IMPORTS: perfumes importados e decants, com pedido pelo WhatsApp.
É um site estático (HTML, CSS e JavaScript puros). Não há build nem dependências.

## Estrutura

```
index.html          página inteira (estilos e script embutidos)
assets/arko-logo.png
favicon.svg
vercel.json
```

## Editar o conteúdo

Tudo fica em `index.html`, no bloco `<script>` no final:

- `WA_NUMBER`: número do WhatsApp com DDI e DDD, só dígitos (ex.: `5561999999999`).
- `WA_LABEL`: número como aparece na página (ex.: `(61) 99999-9999`).
- `PRODUCTS`: lista de perfumes (marca, nome, público, notas e tamanhos com preço).

## Rodar localmente

Abra `index.html` no navegador, ou, na pasta do projeto:

```
python3 -m http.server 8000
```

e acesse http://localhost:8000.

## Publicar no GitHub

```
git init
git add .
git commit -m "Site ARKO IMPORTS"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/arko-imports.git
git push -u origin main
```

## Publicar na Vercel

1. Em vercel.com, clique em **Add New → Project** e importe o repositório do GitHub.
2. Em **Framework Preset**, escolha **Other**. Deixe **Build Command** e **Output Directory** em branco.
3. Clique em **Deploy**.

A cada `git push` na branch `main`, a Vercel publica a nova versão automaticamente.
