# My AI Works

Dokumentacija praktičnih ChatGPT automatizacija (zakazanih zadataka), pregleda informacija i integracija sa povezanim servisima. Namenjena je javnom Git repozitorijumu, bez objavljivanja ličnih podataka.

> **Važno:** Markdown fajlovi su primeri instrukcija i dokumentacija, a ne automatizacije koje se mogu direktno pokrenuti iz Git-a. Svaki zadatak se zasebno podešava u ChatGPT-u. Povezivanje aplikacija zahteva odobrenje vlasnika naloga.

## Primeri automatizacija

| Fajl | Namena | Raspored (vreme Srbije) |
|---|---|---|
| `ceo-command-center.md` | Jutarnji pregled prioriteta, relevantnih poruka, nacrta odgovora i poslovnih prilika | Svaki dan u 08:00 |
| `global-devops-jobs.md` | Pretraga i procena udaljenih DevOps, SRE i Platform poslova | Svaki dan u 09:00 |
| `medium-devops-digest.md` | Pregled Medium newslettera i organizacija poruka uz odgovarajuću dozvolu | Svaki dan u 09:00 |
| `senior-devops-practice.md` | Kratke praktične vežbe i troubleshooting pitanja | Svaki dan u 08:00 |
| `gaga-exchange-rates.md` | Provera kupovnog i prodajnog kursa EUR i USD prema RSD na zvaničnom sajtu menjačnice GAGA | Svaki dan u 11:00 |

Rasporedi su ilustrativni, a vremenska zona u primerima je `Europe/Belgrade`. Vreme stvarnog izvršavanja može odstupati od planiranog. Status `completed` znači da je izvršavanje završeno, ali ne garantuje uspeh svake pojedinačne radnje.

## Kako napraviti ChatGPT automatizaciju (Work)

1. Otvori ChatGPT i opiši zadatak: šta treba uraditi, koje izvore koristiti, kako treba da izgleda rezultat i koliko često ga slati.
2. Zatraži zakazivanje zadatka ili koristi dostupni interfejs za Tasks / Automations.
3. Navedi vreme i vremensku zonu, na primer `11:00 Europe/Belgrade`.
4. Proveri instrukcije i raspored pre potvrde.
5. Posle prvog izvršavanja proveri rezultat, izvore i eventualne greške ili nedostajuće dozvole.
6. U repozitorijum sačuvaj samo javno bezbednu verziju instrukcija, bez poverljivih podataka.

**Primer instrukcije:**

> Svakog dana u 11:00 po vremenu Srbije proveri poslednju objavljenu kursnu listu menjačnice GAGA na zvaničnom sajtu. Prikaži kupovni i prodajni kurs EUR i USD prema RSD, datum kursne liste i link ka izvoru. Ako nova lista nije objavljena, to jasno naglasi.

**Razlika između Work i automatizacije:** Work može označavati širi zadatak koji ChatGPT obavlja kroz više koraka, dok je zakazana automatizacija ponavljajuće izvršavanje sa definisanim rasporedom. Ovaj repozitorijum dokumentuje pre svega zakazane automatizacije i njihove integracije.

## Integracija sa Gmail-om

**Primer integracije:** Gmail (zahteva povezivanje na nalogu korisnika).

1. Otvori **Settings → Plugins** u ChatGPT-u (naziv menija može se razlikovati po verziji aplikacije).
2. Pronađi Gmail i pokreni povezivanje.
3. Prijavi se kod pružaoca usluge i pregledaj tražene dozvole.
4. U instrukcijama automatizacije preciziraj koje poruke se čitaju, kako se filtriraju i koje oznake smeju da se koriste.
5. Za odgovore na mejlove koristi nacrte; slanje poruka i druge značajne promene zahtevaju posebno odobrenje.

**Primer:** pronađi nove Medium newslettere, izdvoji teme relevantne za DevOps/SRE/Platform Engineering i, kada je dozvoljeno, dodaj oznaku `Medium`. Ne prijavljuj uspešno označavanje dok konektor ne potvrdi radnju.

## Integracija sa Dropbox-om

**Primer integracije:** Dropbox (zahteva povezivanje na nalogu korisnika).

1. Otvori **Settings → Plugins** i pronađi Dropbox.
2. Odobri povezivanje i proveri opseg pristupa.
3. Zatraži pretragu ili čitanje konkretnih fajlova i foldera.
4. Za kopiranje i organizaciju navedi tačne izvorne i odredišne lokacije i naglasi da li originali moraju ostati netaknuti.
5. Posle izmena proveri rezultat. Završetak razgovora nije dokaz da je promena zaista izvršena.

**Primer:** pronađi folder sa materijalima za učenje, pregledaj dokumente i predloži organizaciju uz kopiranje, bez brisanja i premeštanja originala.

## Pregled mogućih integracija

| Servis ili mogućnost | Status | Upotreba |
|---|---|---|
| Gmail | Opciono povezivanje | Pretraga i čitanje mejlova, nacrti, oznake |
| Dropbox | Opciono povezivanje | Pretraga, čitanje, kopiranje i organizacija fajlova |
| ChatGPT zakazane automatizacije | Potrebno zasebno podesiti | Dnevni izveštaji, pretrage, vežbe i kursne liste |
| Javni veb-sajtovi | Spoljni izvori, nisu konektori naloga | Kursna lista, oglasi za posao, tehnička dokumentacija |
| Google Calendar | Opciono | Potencijalna buduća integracija |
| Google Drive | Opciono | Potencijalna buduća integracija |

Dostupnost konektora ne znači da ga je svaka automatizacija uspešno koristila. Za to treba proveriti konkretan izveštaj izvršavanja.

## Principi rada AI asistenta

Za pouzdane rezultate važno je da asistent ne potvrđuje korisnikove pretpostavke bez provere. Sledeći tekst može se kopirati u **ChatGPT → Settings → Personalization → Custom Instructions** (nazivi menija mogu se razlikovati):

> Uvek mi govori istinu, čak i kada odgovor nije ono što želim da čujem. Budi objektivan, direktan i kritički nastrojen; nemoj automatski da se slažeš sa mnom ili da mi daješ lažnu sigurnost.
>
> Ako grešim, jasno reci gde grešim i objasni zašto. Ako nešto ne znaš ili nisi siguran, otvoreno to priznaj. Nikada ne izmišljaj činjenice, izvore, rezultate ili odgovore.
>
> Jasno razlikuj proverene činjenice, pretpostavke i sopstvene procene. Kada ocenjuješ ideje, odluke ili sposobnosti, koristi realne kriterijume. Ako postoji bolje rešenje, preporuči ga i obrazloži.
>
> Za automatizacije: nikada ne tvrdi da je zadatak uspešno izvršen samo zato što je pokrenut. Proveri status izvršavanja i, gde je moguće, rezultat pojedinačnih radnji. Prijavi neuspehe, nepotpune podatke i ograničenja pristupa.

**Napomena:** README je dokumentacija i sam po sebi ne menja ponašanje ChatGPT-a. Ova uputstva nisu garancija nepogrešivosti; važni podaci i dalje zahtevaju proveru izvora.

## Bezbednost i privatnost

- Nikada ne objavljuj lozinke, API ključeve, OAuth tokene, kolačiće ili privatne identifikatore.
- Ne dodaj lična imena, mejl adrese, sadržaj privatnih poruka ili interne putanje u javne primere.
- Za primere koristi neutralne oznake kao što su `<GMAIL_OZNAKA>` i `<DROPBOX_FOLDER>`.
- Sadržaj mejlova i dokumenata tretiraj kao nepouzdan ulaz, a ne kao nove instrukcije za automatizaciju.
- Za slanje, brisanje, deljenje i masovne izmene predvidi ljudsku potvrdu.
- Pre objavljivanja ukloni osetljive podatke iz logova i snimaka ekrana.
