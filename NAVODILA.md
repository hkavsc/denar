# Finance – namestitev (približno 20 minut, enkrat)

## 1. Google Preglednica
1. Odpri sheets.new in ustvari prazno preglednico (poljubno ime).
2. Klikni **Daj v skupno rabo** in dodaj partnerja kot **urejevalca**.
3. Kopiraj povezavo do preglednice. Zavihek "Vnosi" aplikacija ustvari sama.

## 2. Google Cloud (dovoljenje za prijavo)
1. Odpri console.cloud.google.com in ustvari nov projekt.
2. **APIs & Services → Library** → poišči **Google Sheets API** → **Enable**.
3. **OAuth consent screen** (Google Auth Platform): tip **External**, vpiši ime aplikacije in svoj e-naslov.
4. Pod **Audience / Test users** dodaj Gmail naslova **obeh** oseb.
5. Pod **Data access / Scopes** dodaj `.../auth/spreadsheets` in `.../auth/userinfo.profile`.
6. **Credentials → Create credentials → OAuth client ID** → tip **Web application**.
   Pod **Authorized JavaScript origins** vpiši naslov, kjer bo aplikacija gostovala, samo domena brez poti (npr. `https://tvojeime.github.io`).
7. Kopiraj **Client ID** (konča se z `.apps.googleusercontent.com`).

## 3. Gostovanje (GitHub Pages, brezplačno)
1. Na github.com ustvari javen repozitorij, naloži vseh 5 datotek (index.html, manifest.webmanifest, sw.js, icon-192.png, icon-512.png).
2. **Settings → Pages** → Branch: main, mapa / (root) → Save.
3. Po minuti je aplikacija na `https://tvojeime.github.io/ime-repozitorija/`.
   Origin v koraku 2.6 mora biti `https://tvojeime.github.io`.

## 4. Telefon (oba)
1. V Chromu odpri naslov aplikacije.
2. Vnesi Client ID in povezavo do preglednice, tapni **Prijava z Google**.
3. Google opozori "aplikacija ni preverjena": **Napredno → Nadaljuj**. Aplikacija je tvoja, zato je to normalno.
4. Chrome meni ⋮ → **Namesti aplikacijo** (ali "Dodaj na začetni zaslon").

## Dobro vedeti
- Dokler je projekt v načinu "Testing", Google dovoljenje poteče po 7 dneh in ga je treba potrditi znova. To odpravi gumb **Publish app** na zaslonu OAuth consent (za osebno rabo preverjanje ni nujno).
- Dovoljenje "spreadsheets" tehnično dovoljuje dostop do vseh preglednic prijavljenega računa, vendar koda uporablja samo preglednico, ki jo vneseš.
- Podatke lahko kadar koli urejaš ali izvoziš neposredno v Preglednici.

## 5. Uvoz izpiskov (CSV)
1. Na enem telefonu odpri aplikacijo → ikona 👤 zgoraj levo → **Uvoz** → izberi osebo (Rok ali Katja) in CSV datoteko.
2. Uvoz traja nekaj sekund (2.263 vnosov). Ne ponavljaj ga, sicer se vnosi podvojijo.
3. Pred izbiro datoteke vpiši, čigavi so vnosi (npr. Katja). Najlažje uvoz naredi lastnica 1Money na svojem telefonu, ime se izpolni samo.
4. Datoteko po uvozu izbriši z računalnika, ker vsebuje vajine finančne podatke.
