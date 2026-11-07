# Limiti e verifica

Verifica documentale del 7 novembre 2026 sul clone del fork. Nessun processo dell'applicazione è stato avviato. Nessun pacchetto è stato installato. Nessun test, build, backtest, benchmark, login, ordine, SSH, sync, merge, deploy o archive è stato eseguito.

Lo SHA head che introduce queste pagine nasce con il commit della PR. La ricevuta con base, head e diff sta nel corpo della PR. Questo file registra la base da cui il ramo è partito: `000a9470cf8461cd8662595bc530993815610b25`.

## Sconosciuto, e lasciato sconosciuto

Identità operativa, uso attuale e investimenti: non accertati. Etichetta del mandato: UNMAPPED. `identity_proven=False`. `unknowncurrentuse=True`. `nextdocscope=unresolved`. `identity_evidence`, `proposalOct`, `decisionlater` e `executionreceipt` sono liste vuote. Queste guide non le compilano.

La descrizione «Trading Agent series» non autorizza accesso a broker, scambi, dati finanziari o associazioni a VPS. Il metadato `parent` dell'API GitHub accerta una genealogia di fork verso `Rizzo-AI-Academy/trading_agent_dashboard`. Non accerta chi usi oggi il fork, su quale host, con quali conti o con quali capitali.

Il linguaggio «non rilevato» è il valore dell'inventario. Nel tree del fork si vedono file `.py`, `.html`, `.json`, `.txt` e `.md`. L'osservazione non corregge l'inventario.

## Contratti, rango, destinatari, condizioni, trigger, host

Cercati per nome nell'elenco dei file del fork e nell'albero pubblico upstream (`truncated=false`). Nessun file di istruzioni root o annidato. Dettaglio e rango M4 nella [matrice](matrice-fonti.md), riga S7. Non è stato aggiunto un rango al posto di quei file.

Trigger solo registrati:

- `templates/dashboard.html`: tre attributi `hx-trigger="load"` sui pannelli `/ui/balance`, `/ui/open-positions`, `/ui/bot-operations`.
- `railway.json`: `restartPolicyType` con valore `ON_FAILURE`, `numReplicas` 1, builder `NIXPACKS`. È presente una stringa `startCommand`. Non è stata eseguita. Nel file non c'è un hostname.

Host non aperti: valore di `DATABASE_URL`, porta e interfaccia citate dal blocco finale di `main.py` (invocazione locale di uvicorn), eventuale destinazione Railway, login Instagram, corpo HTML di Rizzo AI Academy, media YouTube, byte JavaScript e CSS delle CDN. Il controllo sotto registra solo status HTTP.

## Testo presente nel fork, tenuto separato dai risultati

`main.py` descrive l'app, fra le altre parole, come API per leggere dal database Postgres saldo nel tempo, posizioni aperte e operazioni del bot con full prompt, versione stringa `0.3.1`. È una descrizione nel sorgente. Le route GET osservate dai decoratori sono `/balance`, `/open-positions`, `/bot-operations`, `/`, `/ui/balance`, `/ui/open-positions`, `/ui/bot-operations`. Non sono state chiamate. Query, modelli e prompt non sono stati copiati. Un esempio di DSN nel sorgente non è riprodotto qui. Il nome della variabile letta è `DATABASE_URL`; il valore no.

`templates/base.html` contiene questo claim, citato come testo del template e non come identità provata:

> Progetto didattico a cura di Simone Rizzo della serie YouTube «Creo il mio AI trading agent». Tutto il codice dell'agente è disponibile all'interno della Rizzo AI Academy. Per aggiornamenti costanti puoi seguire @simorizzo_ai su Instagram.

Il nome nel template è il nome scritto lì. Non è stato verificato contro un account, un corso o un portafoglio. La serie nominata non è stata guardata. Nessuna strategia e nessuna cifra di performance è stata copiata in queste pagine. Esempi, strategie, prompt e claim non sono policy, non sono risultati certificati e non sono consigli di investimento.

Partial non aperti, nonostante il nome e, per le posizioni aperte, nonostante il blob identico a upstream: `templates/partials/balance_table.html`, `templates/partials/bot_operations_table.html`, `templates/partials/open_positions_table.html`.

Dipendenze dichiarate in `requirements.txt`, non installate: fastapi, uvicorn[standard], psycopg2-binary, python-dotenv, jinja2.

## Fork e upstream

`origin` è `GiacomoGal/trading_agent_dashboard`. Il parent pubblico è `Rizzo-AI-Academy/trading_agent_dashboard` a `4ef19dc92482a027554cb1de8470b714f915a14f`. README upstream, letto via API, è identico alle due righe storiche del fork.

Blob con lo stesso SHA, contenuti non ridiffusi in questa verifica:

| Path | SHA |
| --- | --- |
| `.gitignore` | `b7faf403d915ca307532bb0eb9cceaf0214e8e5b` |
| `README.md` | `02183f7241f2d79b1f5df6db2b8f770d344a3a6d` |
| `railway.json` | `2850b3f631e0df6aa1b91387d85875a686dc88bb` |
| `requirements.txt` | `cb29c98f47d238356f73f5ab083d2504962aa862` |
| `templates/partials/open_positions_table.html` | `6dded33fe4bfbbc062b592985fcdf9784e360e75` |

Blob diversi, byte upstream non scaricati:

| Path | SHA nel fork | SHA upstream | Byte upstream |
| --- | --- | --- | --- |
| `main.py` | `30619ad30304c24112ccb4946703bec6ff59b811` | `c82b0f6f0f4476ac08c5aeccf960f20d0a303e72` | 18250 |
| `templates/base.html` | `e9223b3793537d4b546fab6ea2ee8f6a65454fa7` | `e103d40156d0e23fbf5fec434abb6cd50c20ba3f` | 14109 |
| `templates/dashboard.html` | `d0d461afb17b143ea6af10a4699d99fcef6e37b7` | `f3ef30a3efd738c475f215b902ba3e8e958f737e` | 3696 |
| `templates/partials/balance_table.html` | `8e0eab4ecd5dcd3f1783182ba5010626713995b7` | `494803636d24bb122154726161d6273e4e196dbd` | 4677 |
| `templates/partials/bot_operations_table.html` | `ec3fd7ade732516a07a1c74cec5bd654522898bc` | `92b130e79cc05c74ad8a4bc89f7e1c8a2e010db2` | 3998 |

Path solo upstream, byte non scaricati e non copiati: `check_forecasts.py`, `check_stats.py`, `debug_dates.py`, `debug_snapshots.py`, `forecast_plot_BTC.png`, `forecast_plot_ETH.png`, `forecast_plot_SOL.png`, `inspect_db.py`, `inspect_forecasts.py`, `inspect_forecasts_v2.py`, `inspect_snapshot.py`, `plot_crypto_forecasts_1h.py`, `plot_forecasts.py`, `templates/partials/closed_positions_table.html`, `templates/partials/pnl_stats.html`. Le immagini non sono state aperte. Quei path non sono risultati di forecast di questa guida.

## Link statici

Metodo: GET con `urllib`, timeout 20 secondi, user-agent `doc-link-check/1.0`, handler che non segue i redirect, senza cookie e senza credenziali. Data: 7 novembre 2026. Effetto: una richiesta di status per URL, più un solo hop esplicito dove indicato. Il corpo non è stato interpretato. Gli script non sono stati eseguiti.

| URL nel tree o nel metadato | Esito | Limite |
| --- | --- | --- |
| `https://github.com/GiacomoGal/trading_agent_dashboard` | 200, URL invariato | Pagina pubblica del fork. Non prova uso né investimento |
| `https://github.com/Rizzo-AI-Academy/trading_agent_dashboard` | 200, URL invariato | Pagina pubblica upstream. Non è un merge |
| `https://unpkg.com/htmx.org@2.0.2` | 301 verso il path relativo `/htmx.org@2.0.2/dist/htmx.min.js` | Hop successivo: 200, `Content-Type: text/javascript`. Script non eseguito |
| `https://cdn.jsdelivr.net/npm/chart.js` | 200 | Corpo non eseguito |
| `https://cdn.jsdelivr.net/npm/@picocss/pico@2/css/pico.min.css` | 200 | Foglio non applicato a una pagina |
| `https://www.youtube.com/watch?v=Vrl2Ar_SvSo&list=PLYtHoWz0tONvqawl66HkjgLkEy7xi_6Yp` | 200 | Video e playlist non riprodotti. Nessun claim estratto |
| `http://rizzoaiacademy.com/` | 301 verso `https://rizzoaiacademy.com/` | Hop: 301 verso `https://www.rizzoaiacademy.com/`, poi 200 `text/html`. Corpo non letto. Non è prova di identità o di iscrizione |
| `https://www.instagram.com/simorizzo_ai/` | 302 verso un URL di login Instagram il cui parametro `next` indica il percorso del profilo | Login non seguito. Profilo non aperto. Non è evidenza di identità |

I commenti dentro `.gitignore` citano URL di template Python (Poetry, PDM, gitignore GitHub, Abstra, Cursor). Restano commenti del template. Non sono stati promossi a policy e non sono stati richiesti.

## Effetto di questa verifica

Pagine aggiunte o estese: `README.md`, `AGENTS.md`, `docs/guide/matrice-fonti.md`, `docs/guide/limiti-e-verifica.md`. Nessun altro path del tree va modificato da questa consegna. La review è indipendente. Questo documento non è un PASS.
