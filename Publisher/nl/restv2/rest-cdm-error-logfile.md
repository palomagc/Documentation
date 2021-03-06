# Error registratie in Marketing Suite

Elk bericht dat een error heeft veroorzaakt en is verstuurd vanuit Marketing 
Suite is opgeslagen in de "cdm-error" logfiles. Tijdens het verzenden 
van een emailing kunnen er vele errors voorkomen. De records in deze logfile 
bevatten de beschikbare informatie over deze errors. Je kunt meer lezen 
of errors, ook wel bounces genoemd, in [dit artikel](../bounces). Je kunt de 
inhoud van deze logfile downloaden in CSV, JSON en XML formaat. Zie "Meer informatie 
over logfiles" voor instructies van het opvragen hiervan. De logfiles 
bevatten de volgende informatie.

| Data         | Omschrijving                                        |
| ------------ | --------------------------------------------------- |
| id           | ID van het bericht                                  |
| time         | Tijdstip van rapporteren error                      |
| type         | Type error                                          |
| status       | Status van de error                                 |
| description  | Omschrijving van de error                           |
| code         | Code van de error                                   |
| email        | E-mailadres van de ontvanger                        |
| tags         | Tags van het bericht, gescheiden door puntkomma's   |
| senderdomain | Domein van de verzender                             |
| profile      | ID van het profiel van de ontvanger                 |
| subprofile   | ID van het subprofiel van de ontvanger              |
| template     | ID van de gebruikte template                        |

## Andere logfiles

* [Marketing suite algemeen log](./rest-cdm-attempts-logfile)
* [Marketing suite misbruik log](./rest-cdm-abuse-logfile)
* [Marketing suite click log](./rest-cdm-click-logfile)
* [Marketing suite ontvangst log](./rest-cdm-delivery-logfile)
* [Marketing suite impressies log](./rest-cdm-impression-logfile)
* [Marketing suite herzendingen log](./rest-cdm-retry-logfile)
* [Marketing suite uitschrijvingen log](./rest-cdm-unsubscribe-logfile)
* [Publisher algemeen log](./rest-pom-attempts-logfile)
* [Publisher misbruik log](./rest-pom-abuse-logfile)
* [Publisher clicks (nieuwe stijl) log](./rest-pom-clicks-logfile)
* [Publisher clicks (oude stijl) log](./rest-pom-clicks-logfile)
* [Publisher ontvangst log](./rest-pom-delivery-logfile)
* [Publisher error log](./rest-pom-error-logfile)
* [Publisher impressies log](./rest-pom-impression-logfile)
* [Publisher herzendingen log](./rest-pom-retry-logfile)
* [Publisher uitschrijvingen log](./rest-pom-unsubscribe-logfile)


## Meer informatie over log files

* [Overzicht van alle API calls](rest-api)
* [Vraag namen van logfiles op](rest-get-logfiles-names)
* [Een logfile downloaden in JSON formaat](./rest-get-logfiles-json.md)
* [Een logfile downloaden in CSV formaat](./rest-get-logfiles-csv.md)
* [Een logfile downloaden in XML formaat](./rest-get-logfiles-xml.md)
