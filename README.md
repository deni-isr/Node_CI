# Node.js CI/CD Demo

## Omat lisätoiminnallisuudet

1. **Eristetty MySQL 8.0 -kontti (Service Container):** CI-putkessa käytetään virallista MySQL 8.0 Docker-konttia, jotta tietokanta on aina puhdas ja eristetty jokaista testiajoa varten.
2. **Node.js-versiomatriisi (Multi-version testing):** Testit ajetaan automaattisesti useammalla Node.js-versiolla (18.x ja 20.x) yhteensopivuuden varmistamiseksi.
3. **Automaattinen turvallisuustarkastus (npm audit):** CI-vaiheeseen on lisätty `npm audit` -vaihe, joka tarkistaa riippuvuuksien tunnetut tietoturvaaukot ennen testien ajoa.
4. **Ympäristömuuttujien dynaaminen hallinta:** Tietokantayhteydet ja testausympäristön muuttujat syötetään turvallisesti workflow-tiedoston kautta.


## Ohjeet ja käyttö

- Asenna riippuvuudet: `npm install`
- Aja testit paikallisesti: `npm test`
- CI/CD-putki käynnistyy automaattisesti jokaisesta `git push` -komennosta main-haaraan.