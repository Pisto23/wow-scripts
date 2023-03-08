# Usefull Scripts for Dragonflight

Shows how many charges you have for the catalyst: 
-------------------------------------------------
```
/run local n=(C_CurrencyInfo.GetCurrencyInfo(2167).quantity or 0)print(string.format("Du hast noch %d Aufladungen für deinen Set Katalysator Dings Bums",n,(n==1)and""or"s"))
```

What skill was trained with the Trinket:
----------------------------------------
```
/run for i=2148,2153,1 do V=C_CurrencyInfo.GetCurrencyInfo(i); print(V.name.." - discovered:",tostring(V.discovered)..", quantity:",tostring(V.quantity)) end
```
