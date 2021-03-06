# Data object - message

Het message data-script geeft toegang tot een gepersonaliseerde snapshot van een
[template](./data-object-template). Er kan dus gepersonaliseerde informatie
worden opgevraagd, zoals de broncode en het onderwerp van de message. 

## Beschikbare eigenschappen

* name: 	naam van de snapshot (Read-only property)
* source: 	de broncode van de snapshot (Read-only property)
* subject: 	het onderwerp van de snapshot (Read-only property)
* data: 	zie documentatie over [data data-script](./data-object-data)

## Voorbeeld

Met het volgende voorbeeld in JavaScript kun je de broncode van een gepersonalizeerde template opvragen.

```javascript
var mySourceCode = message.source;
```

## Meer informatie

* [Data-scripts](./data-object)
* [Data data-script](./data-object-data)
* [Template variabele](./data-object-template)
