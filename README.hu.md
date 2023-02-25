# Speciális infrastruktúra webes alkalmazásokhoz

[![en](https://img.shields.io/badge/lang-english%20%F0%9F%87%AC%F0%9F%87%A7-white)](README.md)
[![hu](https://img.shields.io/badge/nyelv-magyar%20%F0%9F%87%AD%F0%9F%87%BA-white)](README.hu.md)

Ez a dokumentum több száz életből vett incidens eredménye.
`#SaaS`

Szolgáltatás nyújtásnál az az irányelvem,
hogy **specializált szolgáltatókat használjunk**, ne népszerűeket, sohasem ingyeneseket.

## WWW

:rock: A Világháló az Internet része,
tehát az Internethez kell kapcsolódnunk, és webes szolgáltatásokat nyújtani.

## Infrastruktúra

- Domain regisztrátor
- DNS szolgáltató
- Szerver szolgáltató
- SSL tanúsítvány kiadó
- CDN szolgáltató
- Tranzakciós email szolgáltató
- Tárterület szolgáltató biztonsági mentéshez

## Prémium szerver szolgáltató

A "felhő" valójában virtualizációt **és** szerver klasztereket jelent.
Sok úgynevezett felhő szolgáltató csak egy fizikai szervert virtualizál.

1. Szoftveralapú **és** redundáns hálózat
2. Szoftveralapú **és** redundáns tároló (storage)
3. Szoftveralapú **és** redundáns szerverek
    (CPU+memória) :point_left: ez nagyon nehéz
4. Vékony azaz hatékony virtualizációs réteg

## Operációs rendszer, middleware, futtatókörnyezet

1. Debian alapon
2. Minden egyes szerver szoftver ismerete, a használaton kívüliek eltávolítása
3. A szerveren lévő minden egyes fájl ellenőrzés alatt tartása (pl. csomagok, git)
4. Kernel, fájlrendszer és minden egyes szerver szoftver
    monitorozása funkcionális tesztekkel, nem csak "pingekkel"

### Middleware

- Apache httpd
- PHP-FPM (FastCGI Process Manager)
- Redis memóriaalapú gyorsítótár
- MariaDB adatbázis

## A webes alkalmazás

Írjunk a lehető legkevesebb forráskódot.
Alaposan tesztelt csomagokra és **specializált** szolgáltatókra építsünk.

- Integrált ügyfélkapcsolat
- Betűtípusok
- Videók
- Térképek
- HTML widget-ek
- Reklám
- Látogató mérés
- fizetés feldolgozó
- Email cím ellenőrzés
- SMS gateway
- Hitelesítés
- Hibakövetés

Az éles környezetek emberi beavatkozás nélkül üzemeljenek.
Minden problémát meg kéne tudni oldani CI-jal
és anonimizált staging környezetekkel.

:bulb: Ismerje fel a technikai adósságát,
amikor kézzel kell dolgozni az éles környezetben.

Havi egyetlen egy _Technikai Adósság Nap_ a stresszt örömmé változtatja.

## Cooperating with providers, software authors

Your application depends on others!

### Analyze your service providers

- Target audience
- Specialized provider vs. populist provider (quality vs. quantity)
- Funds
- Talk to CEO and employees
- Discovery expertise by reading their blog, asking for a demo
- Attitude and tranparency
- Usability
- Infrastructure
- Service providers
- Integrations and API-s
- Price-value ratio

### Know software authors you depend on

- Attitude
- Response to bug reports
- Openness to contributors
- Coverage
- Release frequency
- QA tools in CI