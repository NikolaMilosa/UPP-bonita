# UPP-bonita
Ovde se nalazi Dockerfile za lokalni mailserver kako se ne bi mucili sa googlovim polisama security :D
* Da se izgradi slika:
```
docker build -t mailhog -f Dockerfile
```
* Da se pokrene slika:
```
docker run -p 1025:1025 -p 8025:8025 mailhog
```
* U browseru na `localhost:8025` ce se videti ui za interceptovanje poruka
* Kada se prave connectori za smtp slanje treba :
    1. Postaviti smtp host na locahost
    2. Postaviti port na 1025
    3. Ugasiti tls
    4. From i to su nebitni :)

