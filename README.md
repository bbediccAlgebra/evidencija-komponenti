# Evidento

Evidento je studentski projekt za evidenciju elektroničkih komponenti, planiranje projekata i upoznavanje osnovnih dijelova elektronike.

**Autor:** Borna Bedić, grupa 2OP1

**Kolegij:** AI alati u razvoju softvera

## Organizacija aplikacije

- **Početna** — pregled mogućnosti i objašnjenje tijeka rada.
- **Zalihe** — trenutno stanje, povijest dodavanja i potrošnje te obrasci za promjenu i novu komponentu.
- **Projekti** — ogledni projekti sa statusima, planom dijelova i dosadašnjom potrošnjom te obrazac za novi projekt.
- **Alati** — pristup istraživaču oznaka otpornika.
- **Vodič** — objašnjenja otpornika, kondenzatora i LED diode te česta pitanja.

## Logika evidencije

**Trenutno stanje = početno stanje + dodano − potrošeno.**

Nova komponenta predstavlja novi dio u evidenciji. Dodatne komade postojećeg dijela evidentiramo kao dodavanje. Potrošnju povezujemo s projektom ili općom namjenom.

Planiranje komponenti za projekt ne mijenja zalihe. Količina se smanjuje tek evidentiranjem stvarne potrošnje. Ogledni podaci o zalihama i potrošnji u projektima međusobno su usklađeni.

## Trenutna faza

Projekt je HTML/CSS prototip. Tablice, projektne kartice i rezultati istraživača otpornika unaprijed su napisani u HTML-u.

Forme provjeravaju obavezna polja i dopuštene raspone. Slanje koristi metodu GET: vrijednosti se pojavljuju u adresi stranice, ali se ne spremaju niti ažuriraju prikaz. Gumbi za čišćenje vraćaju početne vrijednosti polja.

Izbornik Zalihe, projektni detalji i česta pitanja rade pomoću oznaka details i summary. Odabir primjera otpornika i pogleda koristi radio polja i CSS selektore :checked i :has(). Prikaz otpornika CSS je ilustracija s dojmom dubine, a ne pravi 3D model.

## Tehnologije i raspored datoteka

- HTML za stranice, navigaciju, tablice i forme.
- CSS Flexbox i Grid za raspored i prilagodbu ekranima.
- CSS tranzicije za promjene boje, položaja i sjena.
- `style.css` sadrži zajedničke stilove.
- `otpornici-stilovi.css` sadrži stilove istraživača i koristi se samo na stranicama Alati i Oznake otpornika.
- `media/` sadrži logo i ilustracije.
- Git i GitHub koriste se za verzioniranje. Veća reorganizacija razvija se u grani `feature/zalihe-projekti-alati`.

Stare datoteke `komponente.html` i `potrosnja.html` zadržane su kao poveznice prema novoj stranici Zalihe. Glavna navigacija ih više ne koristi.

## Pokretanje

Otvori `index.html` u pregledniku ili koristi Live Server u Visual Studio Codeu. Internet je potreban za učitavanje fonta Inter; bez njega koristi se Arial.

## Sljedeća faza

JavaScriptom treba dodati spremanje podataka, stvaranje i brisanje stavki, provjeru potrošnje prema zalihi, povezivanje projekata, filtriranje i učitavanje JSON podataka. Istraživač otpornika kasnije može dobiti slobodan odabir prstenova i automatski izračun.

Za završetak projekta potrebno je postupno pokriti i preostale kriterije projektnog zadatka. Trenutni prototip još ne predstavlja završenu aplikaciju.
