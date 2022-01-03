# VimDocHu
* Ongoing Hungarian Translation of the Vim reference &amp; help files
* A Vim felhasználói kézikönyvének, dokumentációjának (részleges) fordítása

## Állapot
* [x] Kézikönyv: ~100%. 
* [x] Nyelvhelyesség, helyesírási hibák korrekciója, diffmerge folyamatban
* [x] Eredeti fájlok dátuma: 2021.08.25 (összes fájl)

## Teendők
* [ ] Nyelvtani pontosítások
* [ ] Tartalomjegyzék - *.hux fájlok hivatkozásainak konzisztenciája
* [ ] Frissítések implementálása
* [ ] Referencia fájlok átvétele


## A jelenlegi fordítás használatba vétele
* rendelkezz megfelelő jogosultságokkal a `$VIMRUNTIME` mappában
* A VimDocHu/runtime/doc/hu könyvtárat másold be ide: `$VIMRUNTIME/doc`
* A VimDocHu/runtime/syntax/hux.vim fájlt másold be ide `$VIMRUNTIME/syntax`
* töröld a régi tagfájlokat (tags,tags-hu) itt: `$VIMRUNTIME/doc`
* futtasd `:helptags $VIMRUNTIME/doc` a Vimből
* a .vimrchez add hozzá (opcionális):
	* `set helplang=hu,en` (alapértelmezett :help a magyar dokumentációt nyitja
      meg)
	* `syntax on`
	* `au! BufEnter *.hux :set syntax=hux` (ha bemásoltad a syntax filet)
	* `set conceallevel=2`
	* `set concealcursor=n`

## NVIM
* működik, azonban nem ajánlott az Nvim-specifikus differenciák miatt

## Fordítanál?
Az eddig betartott alapelvek:
* Tilos a Google- és egyéb fordítómotorok használata
* A dokumentáció szintaxisát meg kell tartani (|link|,<>, behúzások stb.)
* A fordítás során a magyarosság prioritást élvez a szó szerinti fordításokkal
	  szemben
* Ha úgy érzed, más szavakkal tartalmasabb lenne az információ, fogalmazd át
* Ha úgy érzed, a dokumentáció félreérthetően fogalmaz, pontosítsd
* Ha úgy érzed, hogy a dokumentáció túl szűkszavú, egészítsd ki
* Nem fordítjuk a Vimmel már egybeforrt idegen nyelvű szavakat mint például:
    * quickfix, jumplist, tag, command-line, Insert, Visual, 
    * Replace, shell, autocommand, conceal, fold stb.
* Módosításaidat küldheted pull-requestben, vagy küldd el a
  87.adamtorok@ulster.ac.uk e-mail címre

## Nem fordítanál?
Ebben az esetben az alábbiakban segíthetsz:
* Lefordított szövegek helyesírási hibáinak ellenőrzése
* Lefordított szövegek nyelvhelyességének ellenőrzése
* Hibásan tördelt szövegek javítása
* (help) szintaxis kijavítása

## Ha valami nem tiszta
Egyikünk sem ismeri a Vimet 100%-os pontossággal. A fordítás célja az összes
létező helpfájl lefordítása. Ezért garantáltan lesznek olyan szituációk, melyek
során tesztelni kell a szóban forgó funkcionalitást.
Ha ezek ellenére sem tiszta valami, akkor jelöld meg a kérdéses rész '???'
karakterekkel (ne fordítsd le, vagy ha igen, hagyd meg az angol szöveget is),
hogy könnyedén felderíthető legyen.

## Szerkezet
* `runtime/doc/hu/` - kézikönyv fájljai
* orig/ eredeti fájlok, diffeléshez, karbantartáshoz
* hu.po fájl:
	* a Vim üzeneteit tartalmazza
	* a fájlt a forrással együtt kell lefordítani (teszteléshez is)  `vim/src/po`
	* mielőtt fordítanád (Magyarra) [olvasd el ezt](https://github.com/vim/vim/blob/master/src/po/README.txt)
	* a feldolgozatlan sorok előtt egy globális komment van (üres üzeneteket nem lehet fordítani)
	* push előtt `:source check.vim`-el ellőrizni kell a fjált

## Bugok
* helpgrep magyarul nem működik

 vim:tw=80:filetype=markdown:syntax=markdown
