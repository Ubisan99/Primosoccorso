# 🚑 PrimoSoccorso BLS

> Guida educativa di primo soccorso basata sulle linee guida **ERC / AHA / IRC 2025**.
> Single-file HTML, offline-ready, mobile-first. Nessun framework, nessuna dipendenza, nessun tracking.

![Stato](https://img.shields.io/badge/stato-beta-orange)
![Linee%20guida](https://img.shields.io/badge/linee%20guida-ERC%2FAHA%202025-red)
![Licenza](https://img.shields.io/badge/licenza-MIT-blue)
![Offline](https://img.shields.io/badge/offline-ready-green)
![Lingua](https://img.shields.io/badge/lingua-🇮🇹%20Italiano-green)

---

## ⚠️ Disclaimer importante

**Questa app è materiale educativo. NON è un dispositivo medico. NON sostituisce un corso BLS-D né il consiglio di un professionista sanitario.**

In caso di emergenza reale **chiama sempre il 112**. L'app è pensata come promemoria rapido per chi ha già ricevuto formazione, o come primo approccio informativo per chi non ce l'ha.

> Se stai cercando una certificazione BLS-D valida, rivolgiti a: **IRC (Italian Resuscitation Council)**, **Croce Rossa Italiana**, **ANPAS**, **Misericordie** o centri accreditati regionali.

---

## 🎯 Cosa fa

Una guida rapida a schermo unico che copre le emergenze più comuni in cui un cittadino può trovarsi:

| Sezione | Contenuto |
|---|---|
| ❤️ **RCP** | Sequenza completa adulto/bambino/lattante + metronomo 110 BPM |
| 🫁 **Soffocamento** | Nuova sequenza 2025 (5 pacche + 5 compressioni addominali) |
| 🔥 **Ustioni** | Protocollo raffreddamento + criteri per PS |
| 🛌 **Posizione laterale di sicurezza** | 7 step illustrati |
| 🩸 **Emorragie** | Pressione diretta, bendaggio, laccio emostatico |
| 🔗 **Catena della sopravvivenza** | I 6 anelli ERC 2025 |

---

## 🔑 Caratteristiche

- 📱 **Mobile-first**, pensata per essere usata con una mano in emergenza
- 🔌 **Offline** — nessuna chiamata a server esterni, funziona senza rete
- 📞 **Tel 112 / 118 sempre a portata** in barra fissa
- 🎵 **Metronomo audio + vibrazione a 110 BPM** per le compressioni toraciche
- 🔆 **Wake Lock API** — lo schermo resta acceso durante la RCP
- 🎯 **Zero tracking**, zero cookie, zero analytics
- 📄 **Single file** — apri `primosoccorso.html` in qualunque browser moderno
- 🧠 **Contenuti verificati** su fonti ufficiali aggiornate al 2025

---

## 📚 Fonti

I contenuti sono derivati da linee guida pubbliche e peer-reviewed:

- **ERC Guidelines 2025** — European Resuscitation Council
- **AHA Guidelines 2025 for CPR & ECC** — American Heart Association
- **IRC Italia** — Italian Resuscitation Council
- **ILCOR CoSTR** — International Liaison Committee on Resuscitation

Aggiornamenti chiave 2025 recepiti:

- Soffocamento: **back blows prima delle compressioni addominali** (cambio rispetto a cicli precedenti)
- Chain of Survival unificata a **6 anelli** (include Recovery)
- Conferma **100-120 cpm** / **5-6 cm** profondità per adulti

---

## 🚀 Come si usa

Tre opzioni:

### 1. Scarica e apri
```bash
git clone https://github.com/tuo-username/primosoccorso-bls.git
cd primosoccorso-bls
# Apri primosoccorso.html con il tuo browser
```

### 2. Serve locale (consigliato per Wake Lock)
```bash
python3 -m http.server 8080
# Apri http://localhost:8080/primosoccorso.html
```

### 3. Deploy su GitHub Pages / Netlify / Vercel
Essendo un singolo file HTML, qualsiasi static host funziona out-of-the-box.

---

## 📲 Installazione come PWA (opzionale)

L'app può essere aggiunta alla home del telefono:

- **iOS Safari** → Condividi → *Aggiungi a Home*
- **Android Chrome** → Menu → *Aggiungi a schermata Home*

Si apre a schermo intero come un'app nativa.

---

## 🏗️ Stack tecnico

- **HTML5 + CSS3 + JavaScript vanilla** — nessun framework
- **Web Audio API** — beep del metronomo
- **Vibration API** — feedback aptico
- **Screen Wake Lock API** — schermo sempre acceso durante RCP
- **`tel:` links** — chiamata diretta 112/118
- **~40 KB** totali, zero asset esterni

### Compatibilità browser
| Browser | Supporto |
|---|---|
| Chrome/Edge (Android + Desktop) | ✅ Completo |
| Safari iOS 16.4+ | ✅ Completo |
| Firefox | ✅ Completo (Wake Lock limitato) |
| Samsung Internet | ✅ Completo |

---

## 🎨 Design

- Tema scuro ad alto contrasto (leggibile anche in piena luce o a schermo sporco)
- Tipografia: **Bebas Neue** (titoli), **Space Grotesk** (testo), **DM Mono** (numeri/dati)
- Palette sobria: rosso emergenza (#ff3b3b), ambra avvertimenti, verde conferma
- Icone emoji native — nessun icon pack esterno

---

## 🗺️ Roadmap

- [ ] Supporto multilingua (EN, FR, ES, DE)
- [ ] Modalità PWA installabile con service worker completo
- [ ] Illustrazioni SVG delle manovre
- [ ] Sezione **anafilassi / autoiniettore adrenalina**
- [ ] Sezione **ictus / riconoscimento FAST**
- [ ] Sezione **convulsioni**
- [ ] Versione stampabile A4 per pronto soccorso aziendale
- [ ] Integrazione con app emergenza locali (Where ARE U)

---

## 🤝 Contribuire

Contributi benvenuti, specialmente da:

- Medici, infermieri, soccorritori 118, istruttori BLS-D
- Traduttori madrelingua
- Designer UX per contesti ad alto stress
- Esperti di accessibilità

### Come contribuire
1. Fai fork del repo
2. Crea un branch: `git checkout -b miglioria/nome-breve`
3. Commit delle modifiche con messaggio chiaro
4. Se la modifica è clinica, **cita la fonte** (linea guida, paper, protocollo)
5. Apri una Pull Request

**Modifiche ai contenuti clinici richiedono review da personale sanitario qualificato prima del merge.**

---

## 🐛 Segnalazioni

- **Bug tecnici** → apri una Issue con browser, dispositivo, e passi per riprodurre
- **Imprecisioni cliniche** → apri una Issue con tag `clinical` e **citazione della fonte corretta**
- **Suggerimenti UX** → apri una Discussion

---

## ⚖️ Licenza

**MIT License** — vedi [LICENSE](LICENSE).

Libero uso per scopi personali, educativi e commerciali, con attribuzione. I contenuti clinici sono derivati da linee guida pubbliche dei rispettivi enti; fai riferimento alle fonti ufficiali per uso professionale.

---

## 🙏 Ringraziamenti

A tutti gli istruttori BLS volontari che dedicano il loro tempo libero a insegnare manovre salvavita ai cittadini. Questa app esiste grazie al lavoro di divulgazione di IRC, ERC, AHA e Croce Rossa.

---

## 📬 Contatti

**Autore**: [Lorenzo Leonardo Bortaccio/ @handle]
**Progetto correlato**: [Ubisan99](https://github.com/Ubisan99/Primosoccorso/blob/main) 

---

<div align="center">

**Se questa app può salvare una vita, abbiamo fatto il nostro lavoro.**

🚑 **In emergenza: 112** 🚑

</div>
