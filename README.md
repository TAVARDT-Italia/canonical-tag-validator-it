<p align="center">
  <a href="https://ag.tavardt.com/it/">
    <img src="https://ag.tavardt.com/img/tavardt-banner.png" alt="TAVARDT" width="1024" />
  </a>
</p>

# Validatore di Tag Canonici e Consolidamento di URL

[![Validatore Tag Canonico](https://img.shields.io/badge/TAVARDT-Canonical-5b3cf5.svg)](https://tools.tavardt.com/it/validatore-tag-canonico/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Audit di link canonici, rilevamento di tag duplicati, verifica di URL assolute ed efficienza di scansione.

Sviluppato e mantenuto dalla divisione di ingegneria di indicizzazione e standard tecnici web di **TAVARDT**.

***

## Vettori di Rischio e Impatto Operativo nel Consolidamento di URL

La configurazione erronea dei tag canonici determina cannibalizzazione di pagine e dispersione del ranking sui motori di ricerca. Parametri di tracciamento e filtri di navigazione creano continue repliche della stessa risorsa informativa.

Se le direttive canoniche confliggono tra loro o indirizzano a pagine inesistenti, i bot ignorano il segnale di consolidamento. L audit automatico preserva l autorevolezza del dominio convogliando il posizionamento sulla risorsa primaria.

***

## Funzionalita Centrali di Audit Tecnico

* **Estrazione Direttive da Doppia Sorgente**: Parsing completo di tag canonici dichiarati nell head HTML e nelle intestazioni HTTP Link.
* **Prevenzione Conflitti da Tag Multipli**: Rilevamento immediato di istruzioni canoniche contraddittorie nello stesso documento, con penalita di 35 punti.
* **Verifica URL Assoluto e Protocollo HTTPS**: Validazione di percorsi completi e segnalazione di percorsi relativi o connessioni insicure HTTP.
* **Controllo Attivo Risposta di Destinazione**: Verifica in tempo reale dello stato HTTP della pagina canonica per intercettare errori 4xx o 5xx.
* **Analisi Autoreferenzialita e Consolidamento**: Ispezione di tag autoreferenziali per bonificare parametri di tracciamento e sessione.
* **Indice di Qualita di Consolidamento**: Valutazione tecnica da 0 a 100 che classifica la pagina in COMPLIANT, WARNING o CRITICAL.

***

## Installazione ed Esecuzione

Richiede Python 3.8 o superiore senza dipendenze esterne.

```bash
git clone https://github.com/TAVARDT-Italia/canonical-tag-validator-it.git
cd canonical-tag-validator-it
python canonical_validator.py https://azienda.it
```

Per produrre l output in formato JSON strutturato in pipeline automatiche:

```bash
python canonical_validator.py https://azienda.it -j
```

***

## Domande Frequenti (FAQ Tecnico)

### 1. Cosa accade se su una pagina sono presenti piu tag canonici in conflitto tra loro?
I motori di ricerca ignorano tutte le istruzioni canoniche in presenza di dichiarazioni discordanti sulla stessa risorsa. Cio costringe i crawler a scegliere arbitrariamente l URL da posizionare, frammentando la visibilita.

### 2. Per quale ragione l URL canonico deve essere rigorosamente assoluto e in HTTPS?
I percorsi relativi sono soggetti a errori di interpretazione quando accessibili tramite percorsi virtuali o sottodomini differenti. Inoltre, indicare collegamenti HTTP non protetti genera incongruenze di sicurezza e redirect superflui.

### 3. Quale rischio comporta indicare come risorsa canonica un URL con codice di errore 4xx o 5xx?
Puntare la direttiva canonica verso un URL che restituisce un errore HTTP interrompe il passaggio di autorevolezza. Google disattende il riferimento ed e indotto a indicizzare duplicati non ottimizzati.

### 4. Il software analizza anche le direttive trasmesse nelle intestazioni HTTP Link?
Si, il sistema esamina sia il codice inserito nel head HTML sia le intestazioni HTTP Link del server. Tale prerogativa permette di verificare la corretta canonicalizzazione di documenti statici non HTML come i file PDF.

### 5. In che modo i tag autoreferenziali proteggono le pagine dai parametri di marketing?
Un tag canonico autoreferenziale privo di parametri istruisce i bot a disattendere codici di tracciamento e chiavi di sessione. Questo garantisce che tutte le visite e i segnali di ranking convergano sull URL principale.

***

## Consulenza in SEO Tecnico e Indicizzazione Web

Per architetture web complesse e allineamento agli standard W3C, consultare il team di **TAVARDT**.

***

## Collegamenti Utili

* **Portale Aziendale:** https://ag.tavardt.com/it/
* **Suite di Diagnostica:** https://tools.tavardt.com/it/
* **Contatto Tecnico:** https://ag.tavardt.com/it/contatto/

***

### Licenza
Distribuito con Licenza MIT. Consultare il file LICENSE per i dettagli completi.

***

© 2026 TAVARDT. Tutti i diritti riservati.
