MIJN LOOPCOACH – PWA v3

Functionaliteit:
- 16 weken halve-marathonschema, 3 vaste + 1 optionele looptraining per week
- Trainingsregistratie: datum, status, afstand, duur, gemiddelde hartslag, RPE en notities
- Wekelijkse herstelcheck: benen, vermoeidheid, slaap, motivatie en pijnsignalen
- Persoonlijke tempozones die zich aanpassen aan recente rustige gelogde trainingen
- Dashboard met kilometers per week, gemiddelde hartslag, totalen en belastingsadvies
- Core- en krachtoefeningen met houdingsschetsen en uitleg
- Garmin TCX/GPX-import die afstand, duur, datum en beschikbare hartslag uitleest
- Voorbereiding voor officiële Garmin Connect Activity API / Training API via server-side OAuth 2.0
- Lokale opslag + JSON backup export/import
- PWA/service worker

INSTALLATIE
1. Zet de map op een HTTPS-webserver.
2. Open index.html via de URL op je smartphone.
3. iPhone/Safari: Deel > Zet op beginscherm.
4. Android/Chrome: App installeren / Toevoegen aan startscherm.

GARMIN
TCX/GPX-import werkt zonder API-account. Voor automatische synchronisatie is zakelijke Garmin Developer Program-toegang nodig. Zie server/GARMIN-INTEGRATIE.md.

VERSIE 4
- Volledige 7-daagse weekplanning geïntegreerd.
- Maandag: kracht/core A (algemene loopkracht).
- Dinsdag: looptraining.
- Woensdag: kracht/core B (romp/heupstabiliteit).
- Donderdag: looptraining.
- Vrijdag: lichte core/kracht C (activatie, geen spiervermoeidheid).
- Zaterdag: rust.
- Zondag: lange duurloop.
- Krachtvolume wordt verminderd in herstel-, taper- en wedstrijdweken.


VERSIE 5
- Vandaag toont de echte dagtraining bovenaan.
- Bij kracht/core verschijnen de oefeningen direct met tekening, dosis en uitleg.
- Elke oefening kan afzonderlijk worden afgevinkt.
- De volledige krachtsessie kan met één knop als uitgevoerd worden geregistreerd.
