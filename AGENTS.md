# Guida per agenti — trading_agent_dashboard

Stesso perimetro della [porta d'ingresso umana](README.md). Se una frase di questa pagina e del README divergono, la divergenza è un difetto da rivedere. Non è una licenza per allargare il perimetro. I limiti operativi stanno in [limiti e verifica](docs/guide/limiti-e-verifica.md). La provenienza di ogni affermazione sta nella [matrice](docs/guide/matrice-fonti.md).

## Perimetro

Repository di lavoro: fork `GiacomoGal/trading_agent_dashboard`. Upstream da preservare e da lasciare non unito: `Rizzo-AI-Academy/trading_agent_dashboard`. Base documentata di questa guida: `000a9470cf8461cd8662595bc530993815610b25` su `main`.

La descrizione «Trading Agent series» e il titolo applicativo «Trading Agent Dashboard API» sono testi presenti nel tree. Non autorizzano accesso a broker, scambi, dati finanziari, database, variabili d'ambiente o associazioni a VPS. Identità operativa, uso attuale e investimenti sono sconosciuti (UNMAPPED). `identity_evidence` del mandato resta vuoto. Questa guida non lo riempie.

Nel tree del fork e nell'elenco path dell'upstream non risultano contratti di istruzioni root o annidati (`AGENTS.md` preesistente, `CLAUDE.md`, `CONTRIBUTING`, `CODEOWNERS`, `SECURITY`, `LICENSE`, `.github/`, `.cursor/`, `docs/` preesistente). L'assenza non è una policy nuova, non declassa un contratto e non restringe un rango che non è scritto. Non inventare destinatari, condizioni o trigger al posto di quei file.

## Letture da non fare

Non leggere segreti, `.env`, configurazioni sensibili, backup, memorie, store di agente, account, portafogli, transazioni, dataset privati o record finanziari. Non sincronizzare memorie. Non aprire il valore di `DATABASE_URL`, i corpi dei prompt, le query, i partial di saldo, operazioni e posizioni, né i blob che esistono solo sull'upstream.

I trigger osservati restano chiusi: `hx-trigger="load"` in `templates/dashboard.html` e `restartPolicyType` `ON_FAILURE` in `railway.json`. Nominarli non significa eseguirli. Gli host citati in [limiti e verifica](docs/guide/limiti-e-verifica.md) restano chiusi, oltre il controllo HTTP statico già registrato lì.

## Cosa non è questa pagina

Esempi, strategie, prompt e claim di performance, compresi quelli eventualmente presenti nei file non aperti, non sono policy, non sono risultati certificati e non sono consigli di investimento. Nessuna cifra di performance è stata copiata in queste guide.

La pagina non chiede installazione, import, test applicativi, build, backtest, benchmark, avvio del server, chiamate a broker o provider, login, ordini, SSH, sync, merge, deploy o archive. Non modifica codice, config, script, dati, media o lockfile. Non aggiorna uno stato di lifecycle e non è un PASS.
