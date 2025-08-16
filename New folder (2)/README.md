# PČELARSKA KUĆA DINIĆ — Netlify (Eleventy + Decap CMS)

## Šta dobijate
- Zasebne stranice: /, /products, /gallery, /blog, /videos, /contact
- **Admin samo za vas** preko Netlify Identity + Git Gateway (Decap CMS)
- Blog i Video kao kolekcije — unos preko vizuelnog CMS-a
- Netlify Forms na /contact
- Potpuno responsive (Bootstrap 5)

## Kako postaviti na Netlify
1. Kreirajte **novi Git repo** (GitHub/GitLab/Bitbucket) i push-ujte sadržaj ovog foldera.
2. Na Netlify-u: **Add new site → Import from Git** i povežite repo.
3. Build postavke:
   - Build command: `npm run build`
   - Publish directory: `_site`
4. Deploy.

## Uključite admin samo za vas
1. U Netlify sajtu: **Identity → Enable Identity**.
2. Settings → Identity → Registration: **Invite only**.
3. Kliknite **Invite users** i unesite VAŠ email (samo vi).
4. Settings → Identity → Services → **Enable Git Gateway**.
5. Otvorite `/admin/` na vašem sajtu, ulogujte se preko Netlify Identity i dodajte sadržaj.

## Pisanje sadržaja
- Blog: *Content → Blog postovi* (Markdown fajlovi idu u `content/posts`)
- Video: *Content → Video* (fajlovi u `content/videos`, polje **Embed URL**: npr. `https://www.youtube.com/embed/ID`)

## Kontakt forma
- Poruke stižu u Netlify **Forms** sekciju (naziv forme: `kontakt`).

Srećno! 🐝
