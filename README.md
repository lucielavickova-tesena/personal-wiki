# personal-wiki

Tohle je **nový domov** pro všechny tvoje *osobní* i *sdílené* poznámky.

1. [Použij GitHub šablonu](https://github.com/jan-beranek/personal-wiki/generate) a vytvoř si z ní svůj vlastní centrální repozitář pro poznámky.

Všechny sdílené poznámky z jiných repozitářů si sem pak přidávej jako [[Git Submodules]].
  - [[Tesena-wiki/README|Tesena-wiki]] (https://github.com/Tesena-smart-testing/Tesena-wiki) už je tu pro tebe takto připravena :-)

## Synchronizace
2. Svůj nový repozitář si **naklonuješ** do počítače s přepínači `--recurse-submodules --remote-submodules` a vlezeš dovnitř pomocí `cd`. Například takto:
	```
	git clone --recurse-submodules --remote-submodules git@github.com:jan-beranek/personal-wiki.git
	cd personal-wiki
	```
	- (popřípadě v běžně naklonovaném repozitáři dodatečně stáhneš submoduly:
		`git submodule update --init --recursive --remote`)
3. Přepneš u submodulů, ať začnou **trackovat** svoji main branch:
	```
	git submodule foreach "git checkout main"
	```
4. A **otevřeš** naklonovaný repozitář v aplikaci [Obsidian](http://obsidian.md) jako vault a potvrdíš `Safe mode OFF` (aby fungovaly komunitní pluginy).
    - Předkonfigurovaný Obsidian Git plug-in se pak už postará o automatickou synchronizaci v obou směrech a to včetně vnořených submodulů.
    - (Takže naučit se pracovat s Gitem můžeš opět odložit na jindy... a nebo to může být hned teď první užitečná věc, kterou v Tesena-wiki také najdeš.)
5. **Hotovo**? Fakt? Jo!
   - Tak bež něco dělat a piš si u toho poznámky :-)