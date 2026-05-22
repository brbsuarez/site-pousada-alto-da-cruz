# Site Pousada Alto da Cruz

Site público estático pronto para Cloudflare Pages.

## Cloudflare

- Root directory: `/`
- Build command: `npm run build`

## Arquivos

- `index.html`
- `admin.html`
- `styles.css`
- `script.js`
- `admin.js`
- `firebase.js`
- `config.js`
- `favicon.png`
- `assets/images/`

## Otimização de Imagens

Para converter imagens JPG para WebP via linha de comando (utilizando `cwebp`):

```bash
# Individual
cwebp assets/images/foto.jpg -q 80 -o assets/images/foto.webp

# Em lote (Bash)
for f in assets/images/*.jpg; do cwebp -q 80 "$f" -o "${f%.jpg}.webp"; done
```
