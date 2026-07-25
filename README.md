# Hamster-Lab — GitHub Pages

Landing statica ufficiale (temporanea) di **Hamster-Lab**: brand, teaser ZeroSnob e CTA Buy Me a Coffee. Nessun social inventato.

## Anteprima locale

Apri `index.html` nel browser, oppure dalla cartella:

```bash
cd hamsterlab-site
python3 -m http.server 8080
```

Poi vai su `http://localhost:8080`.

## Aggiorna Buy Me a Coffee

Nel file `index.html` cerca e sostituisci **tutte** le occorrenze di:

```text
https://www.buymeacoffee.com/hamsterlab
```

con il tuo URL reale (es. `https://www.buymeacoffee.com/tuonome`).

Ci sono 3 link (header, hero, sezione supporto).

## Pubblica su GitHub Pages

1. Su GitHub crea un repository **vuoto** (es. `hamster-lab`). Non aggiungere README automatico se preferisci un push pulito.
2. Dalla cartella `hamsterlab-site/` inizializza e pusha il contenuto sulla **root** di `main`:

```bash
cd hamsterlab-site
git init
git add .
git commit -m "Add Hamster-Lab landing for GitHub Pages"
git branch -M main
git remote add origin https://github.com/TUO_USER/hamster-lab.git
git push -u origin main
```

3. Nel repo: **Settings → Pages → Build and deployment**
   - Source: **Deploy from a branch**
   - Branch: **main** / folder **/(root)**
   - Save
4. Dopo 1–2 minuti l’URL sarà tipicamente:

```text
https://TUO_USER.github.io/hamster-lab/
```

5. Incolla quell’URL nel campo **Website** di Buy Me a Coffee.

### Opzione profilo `username.github.io`

Se crei il repo `TUO_USER.github.io`, pusha questi file sulla root di `main`: l’URL sarà `https://TUO_USER.github.io/`.

## Contenuto incluso

- `index.html` — landing
- `styles.css` — stile brand
- `assets/hamsterlab-logo.png` — logo circolare (da `public/HamsterLab_LogoCircular.png`)

## Note

- Nessun build step (HTML/CSS statici).
- ZeroSnob resta “in arrivo”: aggiorna la sezione quando il prodotto sarà online.
