# Uporaba naprave HID

Za razvojno ploščico napišite sistemsko programsko opremo, ki bo demonstrirala uporabo protokola USB HID za miško.

Implementacija naj upošteva naslednje zahteve:

## konfiguracija GPIO priklopov:
- priklop PA0 (modri gumb) kot vhod

## konfiguracija naprave HID:
- opisni niz produkta (PRODUCT_STRING) naj bo "MouseGhost".

## demo miška preprosto:
- ob prvem (lihem) pritisku na gumb zarišite krog z miškinim kazalcem
 - kazalec naj se vrne na začetno mesto
 - premiki naj bodo veliki 31 enot
 - uporabite vsaj 8 premikov
 - časovni zamik med pošiljanjem posameznega premika naj bo 140 ms

## demo miška napredno:
- ob drugem (sodem) pritisku na gumb "simulirajte uporabniško akcijo"
    - premik miškinega kazalca v desno za 419 enot
    - izvedite desni klik
        - pritisnite in spustite desno tipko
    - zavrtite kolesce ("scroll") navzdol za 3 enot
    - izvedite levi klik
        - pritisnite in spustite levo tipko
    - kazalec vrnite na začetno mesto
    - časovni zamik med pošiljanjem posameznega premika naj bo 140 ms
 

Prevedeno sistemsko programsko opremo oddajte v formatu .hex.

V arhivu naloga.zip oddajte naslednjo strukturo:

mapa "Core" (iz korenskega imenika projekta z vsemi podmapami in datotekami)
mapa "USB_DEVICE" (iz korenskega imenika projekta z vsemi podmapami in datotekami)
prevedena sistemska programska oprema (v formatu .hex)