# VimDocHu
* Ongoing Translation of the Vim reference &amp; help files
* A Vim felhasználói kézikönyvének és dokumentációjának részleges fordítása

## Állapot
* A fordítás jelenleg usr_01.hux - usr_07.hux-ig kész (+- pár mondat)
* Folyamatban: usr_08.hux

## A jelenlegi fordítás használatba vétele
* A hu könyvtárat másold be ide: $VIMRUNTIME/doc
* töröld a régi tagfájlokat (tags,tags-hu): $VIMRUNTIME/doc
* futtasd ':helptags $VIMRUNTIME/doc' a Vimből
* a .vimrchez add hozzá ':helplang=hu,en'

## Ha valami nem tiszta
Egyikünk sem ismeri a Vimet 100%-os pontossággal. A fordítás célja az összes
létező helpfájl lefordítása. Ezért garantáltan lesznek olyan szituációk, melyek
során tesztelni kell a szóban forgó funkcionalitást.
Ha ezek ellenére sem tiszta valami, akkor jelöld meg a kérdéses rész '???'
karakterekkel (ne fordítsd le, vagy ha igen, hagyd meg az angol szöveget is),
hogy könnyedén felderíthető legyen.

## Fordítanál?
Az eddig betartott alapelvek:
* Tilos a Google- és egyéb fordítómotorok használata
* A dokumentáció szintaxisát meg kell tartani (|link|,<>, behúzások stb.)
* A fordítás során a magyarosság prioritást élvez a szó szerinti fordításokkal
  szemben
* Ha úgy érzed, más szavakkal tartalmasabb lenne az információ, fogalmazd át
* Ha úgy érzed, a dokumentáció félreérthetően fogalmaz, fogalmazd át
* Ha úgy érzed, hogy a dokumentáció túl szűkszavú, egészítsd ki
* A Vimmel már egybeforrt idegen nyelvű szavakat (mint páldául: quckfix,
  jumplist, tag, command-line, Insert, Visual, Replace stb.) nem fordítjuk

## Nem fordítanál?
Ebben az esetben az alábbiakban segíthetsz:
* Lefordított szövegek helyesírási hibáinak ellenőrzése
* Lefordított szövegek nyelvhelyességének ellenőrzése


vim: tw=80 filetype=markdown syntax=markdown
