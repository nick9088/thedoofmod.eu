---
title: "Come creare una badusb con raspberry pi pico!"
date: 2021-08-28T14:50:28+02:00
draft: false
---
>ATTENZIONE!!!!! VORREI DIRE CHE SE SEGUI QUESTO TUTORIAL DEVI
>USARLO SOLO CON DISPOSITIVI CHE TU POSSIEDI E LO FACCIO SOLO
>PER SCOPI INFORMATIVI, Grazie x l'attenzione!

Quello che ci serve! :

Un Raspberry Pi Pico
Un cavo MicroUSB
Il file UF2 Di CircuitPython
Il driver HID Per CircuitPython
E infine il file python della bad usb

Partiamo!

1. Scarica il file di CircuitPython da qui: https://circuitpython.org/board/raspberry_pi_pico/
2. Trasferisci il file UF2 Appena scaricato nel drive del pi pico
3. Scarica questo archivio: https://github.com/adafruit/Adafruit_CircuitPython_Bundle/releases/tag/20210130
4. Spacchettalo e vai nella cartella lib dell'archivo spacchettato
5. trova nella cartella lib la cartella "adafruit-hid" e trasferiscila in "CIRCUITPY/lib"
6. Scarica questo: https://github.com/dbisu/pico-ducky e scompattalo 
7. Cancella nel drive "CIRCUITPY" il file "code.py" e metti il file "duckyinpython.py" nella root del pi pico e rinominalo "code.py"
8. Adesso crea uno script per rubberducky o scaricane uno da qui: https://github.com/hak5darren/USB-Rubber-Ducky/wiki/Payloads
9. Dopo copia il codice dello script e inseriscilo qui: https://hak5.org/pages/ducky-encoder
10. Clicca "Generate Payload" e "Download DuckyScript" e salvalo come "payload.dd" abilita tutti i file al posto di file di testo
11. Trasferisci il file "payload.dd" nella root del pi pico e appena trasferito rimuovi subito il pi pico altrimenti lo script si avvia

Ce l'avete fatta? Commentate qui sotto per domande! [Devi registrare un account GitHub per commentare]

Ciao!