

**offset entity**
staat in de sectie er boven en wordt het Grid afgetrokken. De gewenste setpoint(range) wordt vervolgens vergeleken met Grid-offset, hier is niets aan verandert wat betreft de werking.

Voorbeelden:
-   Grid +5.000, offset entities+4.000, setpoints 0 0= accu gaat met 1.000 ontladen.
-   Grid +5.000, offset entities+4.000, setpoints 0 800= accu gaat met 200 ontladen.
-   Grid +5.000, offset entities+4.000, setpoints 0 800, Battery Minimum power 500 = accu doet niets want het verschil (200) is lager dan minimum.


**Setpoint targets**
Dit zijn de belangrijkste instellingen voor de aansturing! bij beide 0 invullen is leuk als je nul op de meter wilt maar je kunt er veel meer mee. Omdat ik vermoed dat de meeste NOM willen heb ik daar de defaults instellingen voor ingesteld. In de voorbeelden hieronder staat de rede van -200 +200

- Default: -200 +200 , onder -200 wordt er geladen boven +200 wordt er ontladen. Dit is een dan NOM met een deadband, om zo switchen tussen laden ontladen te verminderen.
- Netsafe: -2.300 +2.300 , binnen de 10 ampere blijven.
- Laden: +10.000 +10.000 , opladen* en max 10.000 totaal van het net.
- Ontladen: -5.000 -5.000 , ontladen* max 5.000* totaal terugleveren aan het net.
- NOM: 0 0 , nul op de meter.

   \* Er van uitgaande dat dit getal hoger/lager is dan je standaard verbruik/opwek.

