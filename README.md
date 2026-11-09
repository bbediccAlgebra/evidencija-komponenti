# Evidento

Evidento je web aplikacija za evidenciju elektroničkih komponenti i praćenje njihove potrošnje. Projekt izrađujem za kolegij **AI alati u razvoju softvera**.

## Stranice

- **Početna** — opis aplikacije.
- **Komponente** — pregled dostupnih komponenti i forma za dodavanje.
- **Potrošnja** — pregled potrošnje i forma za unos potrošenih komponenti.
- **Vodič** — kratka objašnjenja komponenti i česta pitanja.
- **Oznake otpornika** — pet gotovih primjera s promjenom pogleda, objašnjenjem prstenova i tablicom boja.

## Korištene tehnologije

- HTML za strukturu stranica, tablice i forme.
- CSS za izgled, boje, razmake i prilagodbu različitim veličinama ekrana.
- CSS Grid za raspored zaglavlja i kartica.
- Flexbox za navigaciju, kartice početne stranice i raspored elemenata forme.
- CSS tranzicije za postupnu promjenu boja, položaja i sjena.
- Git i GitHub za praćenje verzija projekta.

## Pokretanje

Preuzmi projekt i otvori datoteku `index.html` u pregledniku. Projekt se može pokrenuti i pomoću proširenja Live Server u Visual Studio Codeu.

Za učitavanje fonta Inter potrebna je internetska veza. Bez nje koristi se zamjenski font Arial.

## Trenutno stanje

Izrađene su pet povezanih stranica s prilagodbom za manje ekrane. Forme provjeravaju obavezna polja i dopušteni raspon količine.

Podaci u tablicama zasad su upisani ručno. Spremanje unosa, promjena količina i ostale dinamičke mogućnosti bit će dodani tijekom rada s JavaScriptom.

## Dorade rasporeda i tranzicija

- Početna stranica ima uvod i tri kartice s poveznicama.
- Na stranicama Komponente i Potrošnja tablica je iznad obrasca za unos.
- Polja obrasca koriste Flexbox i prelaze u jedan stupac na mobitelu.
- Obje forme imaju HTML gumb za čišćenje unosa.
- Poveznice iz vodiča otvaraju odgovarajući redak tablice, istaknut CSS selektorom `:target`.

## Istraživač otpornika

Odabir primjera i kuta gledanja radi radio poljima i CSS selektorima `:checked` i `:has()`. Prikaz je CSS ilustracija s dojmom dubine, a rezultati su unaprijed napisani za pet primjera. Nema JavaScripta ni automatskog izračuna. Slobodan odabir svih prstenova i izračun vrijednosti planirani su za JavaScript fazu. Izvor za kodove boja naveden je na stranici.

## Autor

Borna Bedić
