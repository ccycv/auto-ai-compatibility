# Asistent AI nativ în mașină — verificarea compatibilității

**Ghid de eligibilitate, nu kit de instalare.** Scopul este un asistent vocal care rulează pe unitatea multimedia originală, folosește microfonul și difuzoarele mașinii și se conectează la internet prin modemul mașinii, fără telefon sau laptop în utilizarea normală.

Ultima actualizare: **23 noiembrie 2026**. Acesta este un proiect independent, neafiliat producătorilor auto.

> **Nu este o instalare simplă și nu este recomandată ca intervenție DIY.** Evaluarea și adaptarea pot dura ore; pentru o platformă nouă pot necesita mai multe sesiuni de dezvoltare. Procedura diferă după unitate, firmware, echipare și regiune. Fără cunoștințe tehnice de hardware și software există riscul de blocare sau deteriorare a unității multimedia, pierdere a setărilor și necesitatea unei recuperări în service. Un backup nu garantează că recuperarea va fi simplă sau posibilă fără echipament special.

**Aici nu publicăm proceduri de acces la sistem, de modificare, de instalare sau de activare. Nu descărcați și nu instalați pachete pentru a verifica eligibilitatea.**

## 1. Ce este confirmat

| Marcă și model | An / generație | Infotainment testat | Conexiune de date | Ce s-a verificat |
|---|---|---|---|---|
| Audi A4 B9 2.0 TFSI quattro, un singur exemplar de dezvoltare | B9; anul exact al exemplarului nu este publicat | Harman MHI2Q, firmware `MHI2Q_ER_AUG22_P5092`, MU1329 | Conexiune celulară funcțională din MMI, fără hotspot de telefon | Conversație vocală prin microfonul și difuzoarele originale, activare prin apăsare scurtă Voice, indicator pe display și funcții online |

**Confirmarea privește acel exemplar și configurația lui. Nu înseamnă că toate Audi A4 B9 sau toate unitățile cu același firmware sunt deja compatibile.** Accesul la toate datele mașinii, climatizare, camere și alte comenzi nu este promis.

## 2. Modele candidate — necesită verificare și testare

Anii de mai jos sunt **intervale orientative pentru selecția inițială**, nu o listă garantată de echipări. Pot exista suprapuneri între generații, diferențe de piață și unități înlocuite ulterior. **Codul complet al unității și versiunea software au prioritate față de anul mașinii.**

### Platforme apropiate de implementarea existentă

| Marcă | Model / generație | Ani orientativi | Infotainment de căutat | Modul de date necesar | Statut |
|---|---|---|---|---|---|
| Audi | A4 B9, A5 F5 | 2016–2019 / 2017–2019 | MMI Navigation plus Harman, `MHI2_…` sau `MHI2Q_…` | Modem MMI LTE cu SIM/eSIM și date funcționale | De testat pe fiecare exemplar |
| Volkswagen | Golf VII / VII facelift, Passat B8 | aprox. 2015–2020 | Discover Pro **MIB2/MIB2.5 High**, `MHI2_…` / `MHI2Q_…` | Echipare Business/Premium cu modem și SIM, după versiune; se verifică LTE | Candidat; Discover Pro singur nu confirmă generația |
| Škoda | Superb III | aprox. 2015–2020 | Columbus **MIB2 High**, cod complet de verificat | Modul LTE opțional, cu SIM și date active | Candidat |
| Škoda | Kodiaq I | aprox. 2017–2020 | Columbus **MIB2/MIB2.5 High** | Modul LTE opțional, cu SIM și date active | Candidat |
| Porsche | 718 Boxster / Cayman (982) | din 2016, numai exemplare cu PCM4 | **PCM4 / MHI2** | Connect Plus cu modul LTE și SIM/date active | Candidat; anul singur nu confirmă PCM4 |

### Platforma MH2p — adaptare separată

Aceste intervale provin din listele publice de compatibilitate ale platformei; nu reprezintă teste ale asistentului nostru. Căutăm codul **`MH2p_…`**, nu presupunem că orice sistem mai nou este echivalent.

| Marcă | Model / generație | Ani orientativi | Infotainment de căutat | Modul de date necesar | Statut |
|---|---|---|---|---|---|
| Audi | A6 C8, A7 C8, A8 D5, Q8 | 2018–2020 | MIB2+ High / MH2p | Modem de infotainment LTE cu date active | De portat și testat |
| Audi | e-tron, Q3 F3 | 2018–2020 | MH2p, numai dacă este confirmat în versiune | Modem de infotainment LTE cu date active | De portat și testat |
| Volkswagen | Touareg III | 2018–2024 | MIB2+ High / MH2p | Conexiune celulară pentru infotainment | De portat și testat |
| Porsche | 911 (992), Cayenne E3 | 2019–2022 | **PCM5 / MH2p**, nu PCM6 | Modem LTE / Porsche Connect cu date utilizabile de aplicație | De portat și testat |
| Porsche | Macan | 2019–2025, numai exemplare cu PCM5 | **PCM5 / MH2p** | Modem LTE / Porsche Connect cu date active | De portat și testat |
| Lamborghini | Urus | 2018–2023 | LIS III / MH2p | Modem de infotainment cu date active | De portat și testat |

### Alte mărci — cercetare, fără compatibilitate completă demonstrată

| Marcă | Modele de evaluat | Ani orientativi | Infotainment de căutat | Modul de date necesar | Ce rămâne de demonstrat |
|---|---|---|---|---|---|
| BMW | Seria 3 F30/F31, Seria 4 F32/F33/F36 și alte modele echipate cu NBT Evo | în principal 2016–2020; intervalul diferă pe model | **NBT Evo ID5/ID6**, versiune `NBTevo_…`; nu NBT simplu, CIC sau MGU | Modem LTE/telematică compatibil, de identificat individual | Folosirea modemului de aplicație, microfonul, audio și butonul Voice |
| MINI | Hatch F55/F56/F57, Clubman F54, Countryman F60 | aprox. 2017–2020, numai echipări NBT Evo | **NBT Evo**, cod și unitate de confirmat | Modul celular pentru infotainment, dacă există; SIM/date active | Aceleași probe ca la BMW; nu se presupune modem doar din sigla MINI Connected |
| Ford | Focus, Kuga, Mondeo, Mustang și alte modele cu SYNC 3 | aprox. 2016–2021, în funcție de model/piață | **SYNC 3**, versiune și build complete; nu SYNC 4 | Modem LTE / FordPass Connect, dacă este echipat | Accesul aplicației din SYNC la internetul modemului și integrarea vocală |
| Renault | Mégane E-Tech, Austral; Scenic E-Tech și alte modele echipate corespunzător | Mégane/Austral din 2022; Scenic din 2024 | **openR link cu Google built-in / Android Automotive**, nu doar Android Auto | Conectivitate integrată și pachet de date pentru aplicații | Aplicație separată de dezvoltat; accesul root și remaparea Voice nu sunt confirmate |
| Polestar | Polestar 2 | din 2020 | **Android Automotive OS**, versiunea exactă necesară | Modem integrat / Car SIM data, serviciu activ | Aplicație separată de dezvoltat; integrarea Voice și permisiunile trebuie validate |

**Nu sunt incluse automat:** MIB3, Audi MHS2/MST2, MIB2 Standard Delphi, BMW MGU/iDrive 7/8/9, Mercedes MBUX, Volvo Sensus sau orice altă generație nenominalizată. Absența din listă înseamnă „neevaluat”, nu „imposibil”.

## 3. Cum verifici mașina, fără modificări

Parchează și folosește numai meniurile normale de informații. Denumirile pot varia după limbă și firmware. Dacă nu găsești pagina, verifică manualul mașinii sau trimite o fotografie cu meniul principal; **nu intra în meniuri ascunse și nu schimba setări de dezvoltare**.

| Sistem | Unde cauți în meniul normal | Ce fotografiezi / notezi |
|---|---|---|
| Audi MMI | Setări / Settings → informații despre sistem sau versiune / Version information | Pagina completă cu versiunea software, MU și codul unității dacă este afișat |
| VW / Škoda | Setup / Setări → System information / Informații sistem | Hardware, software și numărul unității; dacă nu apare `MHI2`/`MH2p`, trimite ce este afișat |
| Porsche PCM / Lamborghini | Setări → System / informații software sau versiune | Versiunea completă și o fotografie a ecranului principal |
| BMW / MINI | Navigație → Options / Setări → informații despre versiune, dacă există pe acea unitate | Fotografia întregii pagini, inclusiv șirul `NBTevo_…` dacă este afișat; numele hărții singur nu este suficient |
| Ford SYNC 3 | Settings → General → About SYNC | Versiunea SYNC și build-ul complet |
| Renault / Polestar cu Android Automotive | Setări → System → About / Despre | Versiunea Android Automotive și versiunea software a vehiculului; fără identificatori personali |

Nu este necesară desfacerea bordului, scoaterea unității sau conectarea unui tester pentru această evaluare inițială.

## 4. Cum verifici conexiunea de date

Pentru configurația independentă de telefon sunt necesare **modemul mașinii și un serviciu de date activ, utilizabil de aplicație**.

1. Notează dacă există SIM fizic, eSIM, un meniu „Mobile data / Data connection / Car SIM data” sau un abonament de internet pentru infotainment.
2. Deconectează temporar telefonul de la Android Auto/CarPlay și oprește hotspotul telefonului. Verifică să nu fie folosit Wi-Fi-ul casei.
3. Folosește o funcție online nativă disponibilă deja: de exemplu radio online sau o căutare online nouă. Harta deja încărcată și GPS-ul nu demonstrează accesul la internet.
4. Notează dacă funcția merge și ce tip de conexiune indică sistemul. Nu modifica APN-ul și nu activa un abonament nou doar pentru acest test.

**Acesta este doar un test preliminar.** LTE pe ecran, SOS/eCall, controlul mașinii din aplicația producătorului sau un hotspot Wi-Fi nu demonstrează că asistentul nostru poate folosi internetul. Echipa tehnică trebuie să valideze separat accesul aplicației, stabilitatea și reconectarea.

## 5. Ce trimiți pentru evaluare

Copiază și completează:

```text
Marcă și model:
An fabricație / generație:
Piața de origine: Europa / SUA / altă regiune
Infotainment, dacă îl cunoști:
Versiune software completă:
Modul de date: SIM / eSIM / necunoscut
Internetul nativ merge fără telefon și fără Wi-Fi extern: da / nu / netestat
Buton Voice pe volan: da / nu
Unitatea multimedia a fost înlocuită sau modificată: da / nu / nu știu
```

Atașează o fotografie a meniului principal și una cu versiunea software. Trimite-le persoanei care ți-a oferit acest link, prin canalul privat deja folosit.

**Nu publica VIN-ul complet, IMEI, ICCID, numărul SIM, parole, coduri de activare, locația personală sau datele contului.** Acoperă aceste câmpuri în fotografii. Nu deschide un issue public cu date personale.

## 6. Ce se întâmplă după verificare

Evaluare a echipării → verificare tehnică individuală → estimare a lucrării → backup și plan de recuperare → adaptare și test supravegheat, numai cu acordul proprietarului.

O unitate eligibilă nu înseamnă instalare garantată. Accesul la sistem, internetul, microfonul, difuzoarele, butonul Voice, pornirea automată și datele vehiculului se validează separat. Nu promitem controlul tuturor funcțiilor mașinii și nu solicităm modificări ale sistemelor de siguranță.

**Nu face update sau downgrade de firmware pentru a „te potrivi” cu lista.** Trimite întâi versiunea existentă. Acest repository nu oferă fișiere de instalare, firmware, metode de deblocare sau instrucțiuni de modificare.

[Surse și limitele listei](SOURCES.md)
