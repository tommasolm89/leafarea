# 🌿 LeafArea Pro

**App web per il calcolo dell'area fogliare** con rilevamento automatico dei bordi del foglio.

## 🎯 Funzionalità

- 📷 **Scanner con rilevamento automatico** - Rileva automaticamente i bordi del foglio
- 🔧 **Regolazione manuale** - Aggiusta i 4 angoli trascinandoli
- 📐 **Trasformazione prospettica** - Raddrizza automaticamente l'immagine
- 🎨 **Calibrazione colore HSV** - Regola le soglie per lo sfondo
- 📊 **Calcolo area fogliare** - Risultato in cm²
- 💾 **Storico misurazioni** - Salva e esporta in CSV
- 📱 **PWA** - Installabile come app sul telefono

## 🚀 Come usare

1. Apri l'app da un browser (Chrome consigliato)
2. Imposta le dimensioni della superficie di riferimento (es. 100x140 cm)
3. Scatta una foto del foglio con le foglie appoggiate
4. Regola i bordi se necessario
5. Clicca "Analizza area fogliare"

## 📐 Principio di funzionamento

L'app calcola l'area fogliare usando il metodo della **superficie di riferimento nota**:

```
Area fogliare = (pixel foglie / pixel totali) × Area superficie
```

Lo sfondo colorato (es. magenta) viene filtrato tramite soglie HSV, e tutto ciò che non è sfondo viene considerato "foglia".

## 🔧 Calibrazione

Per ottenere risultati accurati:

1. Vai nella tab **Calibra**
2. Carica un'immagine di esempio
3. Tocca lo sfondo per campionare il colore
4. Regola gli slider HSV se necessario
5. Salva la calibrazione

## 💡 Suggerimenti

- Usa uno sfondo di colore uniforme e contrastante (magenta funziona bene)
- Assicurati che l'illuminazione sia uniforme
- Inquadra l'intero foglio di riferimento
- Per lo scanner in tempo reale serve HTTPS (GitHub Pages lo fornisce)

## 🛠️ Tecnologie

- HTML5 / CSS3 / JavaScript (ES5 per compatibilità)
- [OpenCV.js](https://docs.opencv.org/) per rilevamento bordi e trasformazione prospettica
- LocalStorage per persistenza dati

## 📄 Licenza

MIT License - Libero per uso personale e commerciale.

---

Sviluppato per ricerca agricola 🌱
