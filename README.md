# Projekt célja
Adózási szempontból átlátható és követhető a befektetések értéke.

# Használati útmutató
1. main.py és wallet_data.xlsx letöltése
2. Excel táblázat első 3 oszlopának kitöltése:
    * A oszlopba kerül a kriptovaluta neve
    * B oszlopba kerül a vételi árfolyam
    * C oszlopba kerül a vásárolt mennyiség
3. A main.py lefuttatása után a terminálba megjelenik a jelenlegi árfolyam és a nyereség/veszteség %-os formában
4. A program automatikusan frissíti az excel tábla hiányzó mezőit

# Működési elv
A program a szükséges adatokat a [CoinMarketCap](https://coinmarketcap.com/) nevű oldalról gyűjti be API segítségével.   
A számításokhoz szükséges információkat egy listában elmentjük.    
Bekérjük az excel táblázatban szereplő kriptovaluták nevét és kikeressük a hozzájuk tartozó aktuális árfolyamot.    
Az excel frissítése 2 listát használunk:   
* list_for_update_excel lista menti a keresett árfolyamokat.   
* profit_loss lista menti a nyereség/veszteséget %-os formában. 
