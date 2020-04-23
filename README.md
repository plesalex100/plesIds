# plesIds
Afiseaza buletinul / permisul romanesc

### Usage (Server Side)

Functia pentru a afisa buletinul:
folositi functiile vRP.getUserIdentity() si vRP.getUserAddress() pentru a lua numele, anii si adresa
```
TriggerClientEvent("ples-id:showBuletin", player, {nume = firstname, prenume = name, age = age, adresa = home.." Nr. "..number, usr_id = nuser_id, target = playerSource})
```

Functia pentru a afisa permisul:
```
vRP.getUserIdentity({nuser_id, function(identity)
  TriggerClientEvent("ples-id:showPermis", player, {nume = identity.firstname, prenume = identity.name, target = nplayer})
end})
```

### FAQ
- Comenzile de mai sus se pun oriunde doriti ca buletinul/permisul sa fie afisat
- Aceasta resursa a fost postata gratis deoarece au existat tentative de vanzare la aceasta resursa, de aceea nu ofer support pentru aceasta resursa, aveti informatiile necesare mai sus.
