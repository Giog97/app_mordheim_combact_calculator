# ⚔ Mordheim Combat Calculator - PWA

https://giog97.github.io/app_mordheim_combact_calculator/

## Come installare sul telefono

### Android (Chrome)
1. Apri `index.html` su un server web (vedi sotto) con Chrome
2. Tocca i tre puntini in alto a destra → **"Aggiungi a schermata Home"**
3. Conferma → l'app appare come icona sul desktop

### iPhone / iPad (Safari)
1. Apri `index.html` con Safari
2. Tocca il tasto **Condividi** (quadrato con freccia in su)
3. Scorri e tocca **"Aggiungi a schermata Home"**
4. Conferma

---

## Come pubblicare i file (opzioni gratuite)

### Opzione 1 — GitHub Pages (consigliata)
1. Crea un account su [github.com](https://github.com)
2. Crea un repository pubblico, es. `mordheim-app`
3. Carica i tre file: `index.html`, `manifest.json`, `sw.js`
4. Vai in *Settings → Pages → Source: main branch*
5. L'app sarà disponibile su `https://tuonome.github.io/mordheim-app/`

### Opzione 2 — Netlify Drop
1. Vai su [app.netlify.com/drop](https://app.netlify.com/drop)
2. Trascina la cartella con i tre file
3. Ottieni subito un URL pubblico tipo `https://random-name.netlify.app`

### Opzione 3 — Server locale (solo WiFi casa)
```bash
# Con Python 3 installato:
cd cartella-mordheim
python3 -m http.server 8080
# Poi sul telefono (stesso WiFi): http://IP-DEL-PC:8080
```

---

## Funzionalità
- **Schermo sempre attivo** tramite Wake Lock API (indicatore verde in alto)
- **Offline** dopo la prima visita (Service Worker)
- **Installabile** come app nativa (PWA)
- Calcolo mischia, tiro e tabelle di riferimento complete

## File inclusi
| File | Descrizione |
|------|-------------|
| `index.html` | App completa |
| `manifest.json` | Metadati PWA per l'installazione |
| `sw.js` | Service Worker per il funzionamento offline |

> Nota: per l'icona dell'app, aggiungi due file PNG nella stessa cartella:
> `icon-192.png` (192×192px) e `icon-512.png` (512×512px).
> Senza icone l'app funziona lo stesso, ma usa un'icona generica.
