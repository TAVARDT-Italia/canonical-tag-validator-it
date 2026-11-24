# Validatore di Tag Canonico e Consolidamento URL

[![Validatore Tag Canonico](https://img.shields.io/badge/TAVARDT-Canonical-5b3cf5.svg)](https://tools.tavardt.com/it/validatore-tag-canonico/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)

Verifica tecnica di URL canonici, prevenzione della duplicazione dei contenuti e conformita W3C.

Sviluppato e mantenuto dalla divisione di architettura semantica e indicizzazione di **TAVARDT Italia**.

***

## Funzionalita di Verifica Tag Canonico

* **Rilevamento Direttive Canoniche**: Ispezione della presenza di `<link rel="canonical">` nell'intestazione HTML e negli header HTTP.
* **Prevenzione Tag Multipli**: Segnala la presenza di tag canonici multipli e conflittuali all'interno dello stesso documento.
* **Convalida Percorsi Assoluti**: Assicura l'utilizzo di percorsi assoluti con protocollo sicuro HTTPS.
* **Verifica Codice di Risposta del Destinatario**: Controlla che l'URL canonico di destinazione restituisca lo stato HTTP 200 OK.
* **Punteggio di Salute di Indicizzazione**: Metrica quantitativa da 0 a 100 con passaggi tecnici di ottimizzazione.

***

## Installazione ed Esecuzione

Richiede Python 3.8 o superiore, basato esclusivamente sulla libreria standard.

```bash
git clone https://github.com/TAVARDT-Italia/canonical-tag-validator-it.git
cd canonical-tag-validator-it
python canonical_validator.py https://azienda.it
```

Per generare il rapporto in formato strutturato JSON:

```bash
python canonical_validator.py https://azienda.it -json
```

***

## Diagnostica Completa sul Web

Per verifiche estese di consolidamento canonico:

* **Validatore di Tag Canonico Ufficiale**
* **[Portale Aziendale TAVARDT Italia](https://ag.tavardt.com/it/)**

***

## Consulenza in Indicizzazione e SEO Tecnico

Per progetti di architettura web conformi a Standard W3C e Linee Guida AgID, contattare il team di **TAVARDT Italia**.

***

© 2026 TAVARDT. Tutti i diritti riservati.
