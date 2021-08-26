# VimDocHu
Ongoing Translation of the Vim reference &amp; help files

## How to configure
* Please move the 'hu' directory into your $VIMRUNTIME/doc
* remove tags (and) tags-hu files from $VIMRUNTIME/doc
* run ':helptags $VIMRUNTIME/doc in vim'
* Add to your .vimrc to prioritize hu help files ':helplang=hu,en'
* search the original documentation if needed like :h tag@hu

## If something is not clear
* mark that with an '???' and leave the whole sentence and/or section untranslated and we will figure that out (mostly caused by language barrier)
* mark that with an '@@@' where the English is okay but you do now how the things work in Vim
* If you want, add your comment as well like:
    * "??? My Comment ???"
    * "@@@ Mz comment @@@"
    * Or even your translation but in this case leave the original text intact

## PLease only commit if
* Your English better than good
* Your Hungarian grammar is nearly perfect
* You not gonna use translate engines
* You understand the meaning of the english information and you are not afraid to void the 'word by word' translation sometimes

