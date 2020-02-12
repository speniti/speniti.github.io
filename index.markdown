---
layout: default
---
# Curriculm Vitae
---
## Esperienza professionale

{% for job in site.data.jobs %}
| | |
| ---: | --- |
| **Data** | {{ job.date }} |
| **Posizione ricoperta** | {{ job.position }} |
| **Attività e responsabilità** | {{ job.activity }} |
| **Nome e indirizzo datore di lavoro** | {{ job.company.name }}<br>{{ job.company.address }} |
{% endfor %}

## istruzione e formazione

{% for school in site.data.schools %}
| | |
| ---: | --- |
| **Data** | {{ school.date }} |
| **Qualifica rilasciata** | {{ school.certificate }} |
| **Nome dell'organizzazione** | {{ school.organization.name }}<br>{{ school.organization.address }} |
{% endfor %}

### Lingue

|                  |          |
| ---------------: | -------- |
|  **Madrelingua** | Italiano |
| **Altre lingue** | Inglese  |

## Capacità e competenze
{% for competency in site.data.competencies %}
| {{ competency.name }} |
| --- | 
| {% for value in competency.values %} {{ value }}<br> {% endfor %} |
{% endfor %}

## Altri progetti

- Creazione e gestione di una web radio.
- Sviluppo di un applicativo gestionale utilizzando i framework Laravel e Vue JS.
- Sviluppo di una progressive web app.

## Patente

A e B, auto/moto munito.  

> Autorizzo il trattamento dei dati personali contenuti nel mio curriculum vitae in base all’art. 13 del D. Lgs. 196/2003 e all’art. 13 GDPR 679/16.