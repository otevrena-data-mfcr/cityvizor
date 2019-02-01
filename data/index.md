---
layout: default
title: Data
menu: data
---

* TOC
{:toc}

## REST API

CityVizor nabízí jednoduché API pro stahování exportů dat. Toto API bude postupně vylepšováno dle požadavků uživatelů dat.

Vlastnosti dat:
- v současnosti neexistuje limit na stažení dat, v případě zneužívání exportů bude zaveden
- data jsou s maximálně hodinovým zpožděním
- data jsou exportována ve formát JSON

Všechny žádosti jsou na endpoint ```cityvizor.cz/exports/v1```.

### Profily obcí

```GET /profiles```

### Profil obce

```GET /profiles/:profile```

### Datové sady profilu obce

```GET /profiles/:profile/etls```

### Rozpočty obce

```GET /profiles/:profile/budgets```

### Rozpočet obce za rok

```GET /profiles/:profile/budgets/:year```

### Faktury obce za rok

```GET /profiles/:profile/payments/:year```
