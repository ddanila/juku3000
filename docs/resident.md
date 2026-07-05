# Juhend residentsete programmide laaduri `JLOAD.LDR` kasutamiseks.

1.  Residentseks tehtav programm peab  sisaldama
    unikaalset identifikaatorit, mille järgi tehakse
    kindlaks, kas programm juba pesitseb mälus või
    mitte. Identifikaator peab paiknema neljanda
    baidina programmis. Näiteks:
   
    ```
    START:: jmp   INIT
    ID:     db    08h  ; Identifikaator
    INIT:   mov .....  ; Programm ise
            .
            .
            .
    ```

2.  Programm transleerida `M80`-ga, seejärel linkida
    `LINK`-iga, kasutades `[op]` võtit.
    Näit:

    ```
    M80 DRIVER.ERL=DRIVER.MAC
    LINK DRIVER.ERL [op]
    ```

    Kui `LINK` on töö lõpetanud, võib kettalt leida
    `.PRL` laiendiga faili.

3.  Saadud `.PRL` laiendiga fail tuleb ühendada 
    residentsete programmide laaduriga `JLOAD.LDR`
    `SID`-i abil. Selleks tuleb `SID`-i alt laadida
    `JLOAD.LDR` ja seejärel residentne  programm
    (`.PRL` laiendiga) aadressile `167h`. Näiteks:

    ```
    A>sid

    #ijload.ldr
    #r
    #idriver.prl
    #r167
    ```
    
    Nüüd on mälus laadur koos laetava programmiga
    st. lõplik  programm, mis tuleb salvestada
    kettale CP/M käsu `SAVE` abil. Salvestatava
    koguse võib teada saada, vaadates `SID`-i alt
    mälu sisu.  Kuna `.PRL` fail lõpeb suurema koguse
    hex `1A`-dega, siis on programmi lõppu üsna
    lihtne kindlaks teha. Kui on selge, kui palju
    on vaja kettale kirjutada, tuleb `SID`-ist 
    väljuda  (`CTRL-C`) ja salvestada lõplik 
    programm kettale juba `.COM` laiendiga. Näit.:

    ```
    A>save <n> driver.com
    ```


