# Infocesty – terénny zápisník · návod na spustenie

**Primatour s.r.o.** · verzia 0.2 · 11. 9. 2026

Zápisník je jednoduchá webová appka do telefónu. Funguje bez internetu, všetko si pamätá v telefóne a na konci cesty jedným tlačidlom vyexportuje poznámky, odpovede aj hlasové nahrávky.

---

## 1. Nahratie na web (raz)

Appka musí bežať na adrese so zámkom (https), inak telefón nepovolí mikrofón a ukladanie bez internetu. Web www.primatour.sk hostuje **Cesys (cestovnysystem.sk)**, preto nahratie robia oni.

1. V administrácii Cesysu kliknite vľavo dole na **„CeSYS podpora"** (alebo im napíšte e-mail) a pošlite im balík `infocesty-zapisnik-v0.2.zip` s prosbou: rozbaliť obsah do nového priečinka **`infocesty`** v koreňovom adresári webu tak, aby fungovala adresa **https://www.primatour.sk/infocesty/index.html**. Je to samostatná statická stránka na interné použitie, do systému nezasahuje.
2. V balíku je 6 súborov, ktoré majú byť v priečinku: `index.html`, `sw.js`, `manifest.webmanifest`, `hotels.json` (zoznam hotelov z ponuky Cesys – našepkávanie názvov), `icon-192.png`, `icon-512.png`. Súbor `NAVOD.md` je len tento návod.
3. Keď potvrdia, otvorte **https://www.primatour.sk/infocesty/** – mala by sa zobraziť čierna hlavička PRIMATOUR a formulár „Nová infocesta".

> Poznámka: priečinok `infocesty` nie je nikde na webe prelinkovaný, takže ho bežný návštevník nenájde. Nie je chránený heslom – v zápisníku sú len vaše poznámky v telefóne, na server sa nič neukladá.

## 2. Pridanie na plochu telefónu (každý člen tímu, 1 minúta)

**iPhone (Safari):** otvorte adresu v Safari → dole tlačidlo **Zdieľať** (štvorček so šípkou) → **Pridať na plochu** → Pridať. Na ploche pribudne žltá ikona „Infocesty".

**Android (Chrome):** otvorte adresu v Chrome → menu ⋮ vpravo hore → **Pridať na plochu** / **Inštalovať aplikáciu** → Pridať.

Odteraz appku otvárajte **len z tejto ikony**, nie z prehliadača. Vtedy funguje bez internetu a dáta sa nemažú.

## 3. Prvé použitie

1. Otvorte ikonu, vyplňte **názov cesty** (napr. „Rodos, september 2026"), termín a kto zapisuje → **Založiť cestu**.
2. Ak máte program, pridajte hotely do zoznamu: začnite písať názov a appka ponúkne hotely z ponuky Cesys aj s letoviskom a kódom – ťuknite na správny. Hotel, ktorý v ponuke nie je, stačí pomenovať. Ak program nemáte, pridáte hotely až na mieste rovnakým spôsobom.
3. Pri prvej nahrávke sa telefón spýta na povolenie **mikrofónu** → Povoliť.

## 4. V hoteli

- Hore vždy vidíte **„SOM V HOTELI"** – všetko sa ukladá k tomuto hotelu. Pri ďalšom hoteli ťuknite **Prepnúť**, vyberte zo zoznamu alebo napíšte nový názov.
- **Body**: napíšte pár slov, Enter. Štítok vpravo (izby, pláž…) sa dá ťuknutím zmeniť, nemusíte.
- **Nahrať poznámku**: ťuknite, hovorte, ťuknite znova. Nahrávka sa uloží k hotelu; prepíšeme ju po návrate.
- **Checklist**: otázky klientov, klikáte možnosti. Pri niektorých sa dá vybrať viac.
- **Prejsť hotel krok za krokom**: sprievodca (prvý dojem → izby → pláž → jedlo → okolie → záver), keď máte čas, napr. v autobuse.
- **Fotky**: foťte bežným fotoaparátom telefónu. Appka si pamätá časy, kedy ste boli v ktorom hoteli – fotky spárujeme podľa nich. Nič netriedte.

## 5. Večer

Záložka **Deň** ukáže, ktoré hotely ste dnes videli a kde chýba checklist alebo body. Ťuknutím doplníte.

**Odporúčam každý večer urobiť export** (záložka Cesta → „Odoslať / uložiť export") a poslať si ho na e-mail alebo do Google Drive. Je to záloha pre prípad, že by sa s telefónom niečo stalo. Exportovať sa dá koľkokrát chcete, nič sa nezmaže.

## 6. Po návrate

Záložka **Cesta** → **Odoslať / uložiť export (s nahrávkami)**. Telefón otvorí okno „Zdieľať" – pošlite dva súbory (`.txt` a `.json`) e-mailom alebo ich uložte do Google Drive a pošlite mi ich. Z nich vzniknú karty hotelov.

Potom môžete cestu **Uzavrieť** – dáta ostanú v telefóne, len sa pripraví miesto na ďalšiu cestu.

## 7. Čo zápisník (zatiaľ) nerobí

- Neprepisuje hlas na text – to sa urobí po návrate.
- Nepriraďuje fotky sám – foťte fotoaparátom, spárujú sa podľa času.
- Nesynchronizuje sa medzi telefónmi – každý má svoje dáta a pošle export.
- Nemá heslo – nedávajte doň nič citlivé.

Toto všetko príde v plnej verzii appky. Zápisník je prvý krok, aby sme z najbližšej cesty mali skutočné dáta.

## 8. Keď niečo nejde

- **Mikrofón nefunguje** → skontrolujte, či je adresa s https a či ste povolili mikrofón (Nastavenia telefónu → Safari/Chrome → Mikrofón).
- **Appka je prázdna po otvorení** → otvorili ste ju z prehliadača namiesto z ikony na ploche? Dáta sú v ikone.
- **Export sa neotvorí** → skúste „Export len text a odpovede" (menší súbor) a nahrávky pošlite neskôr z wifi.
- Čokoľvek iné → snímku obrazovky a napíšte mi.
