# Curtea Veche — Jibou

Site de prezentare pentru restaurantul tradițional românesc **Curtea Veche**, Strada Parcului nr. 2, Jibou.

**Live:** https://danmarius9611.github.io/curteavechejibou/

## Structură

| Fișier | Rol |
|---|---|
| `index.html` | Pagina publicată — o singură pagină, CSS și JS inline, imagini locale din `img/` |
| `curtea-veche-design_1.html` | Fișierul de design original, cu imaginile servite de pe CDN-uri externe |
| `img/` | Imaginile paginii (fotografii restaurant + fotografii de stoc pentru preparate) |

## Dezvoltare

Nu există build step — este HTML static. Deschide `index.html` direct în browser, sau pornește un server local:

```bash
python -m http.server 8000   # sau: npx serve .
```

Orice push pe `main` se publică automat prin GitHub Pages.

## De înlocuit înainte de lansare

- Fotografiile de preparate din `img/` sunt imagini de stoc (Unsplash) — de schimbat cu poze reale.
- Formularul de rezervare este doar vizual; nu trimite nimic. Necesită backend sau un serviciu tip Formspree.
