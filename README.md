# Node.js CI/CD Demo

## Omat lisätoiminnallisuudet

1. **Oma MySQL-kontti tietokannalle:** CI ajaa virallista MySQL 8.0 Docker-konttia, jotta tietokanta on aina tyhjä ja puhdas jokaista testiajoa varten.
2. **Testaus eri Node-versioilla:** Testit ajetaan automaattisesti useammalla Node.js-versiolla (20.x ja 22.x), jotta nähdään koodin toimivan varmasti eri ympäristöissä.
3. **Automaattinen turvatarkastus:** CI-putkeen kuuluu npm audit vaihe, joka tsekkaa pakettien tunnetut tietoturvaaukot ennen testien ajamista.
4. **Ympäristömuuttujien hallinta:** Tietokanta asetukset ja muut muuttujat syötetään turvallisesti suoraan workflow-tiedoston kautta, eikä niitä tarvitse kovakoodata sovelluksen koodiin.

## Ohjeet ja käyttö

Asenna riippuvuudet: `npm install`
Aja testit paikallisesti: `npm test`