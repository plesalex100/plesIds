# plesIds
Afiseaza buletinul / permisul romanesc

### Usage (Server Side)

Functia pentru a afisa buletinul:
```lua
-- param @player = Number: Source-ul player-ului caruia i se afiseaza pe ecran
-- param @firstname @name @age @home @number = String: datele jucatorului care va aparea in buletin
-- param @target_id = Number: Id-ul jucatorului care va aparea in buletin
-- param @target_src = Number: Source-ul jucatorului care va aparea in buletin

TriggerClientEvent("ples-id:showBuletin", player, {
  nume = firstname, 
  prenume = name, 
  age = age, 
  adresa = home.." Nr. "..number, 
  usr_id = target_id, 
  target = target_src
})
```

Functia pentru a afisa permisul:
```lua
-- param @nuser_id = Number: Id-ul jucatorului care va aparea in buletin
-- param @player = Number: Source-ul player-ului caruia i se afiseaza pe ecran
-- param @nplayer = Number: Source-ul jucatorului care va aparea in buletin

vRP.getUserIdentity({nuser_id, function(identity)
  TriggerClientEvent("ples-id:showPermis", player, {
    nume = identity.firstname, 
    prenume = identity.name, 
    target = nplayer
  })
end})
```

### Poze
![alt text](https://i.imgur.com/UTQ9xtE.png) 
![alt text](https://i.imgur.com/66TC32K.png)

FAQ
-

- Comenzile de mai sus se pun oriunde doriti ca buletinul/permisul sa fie afisat
- Aceasta resursa a fost postata gratis deoarece au existat tentative de vanzare la aceasta resursa, de aceea nu ofer support pentru aceasta resursa, aveti informatiile necesare mai sus.
