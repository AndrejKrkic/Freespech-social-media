Projekat sadrži dve aplikacije radjene u Node.js-u i React-u. Sledi detaljan opis i redosled izvršavanja naredbi za uspešno pokretanje projekta.
Koraci za pokretanje:
1. Preuzeti projekat(u ZIP ili nekom drugom formatu), otpakovati ga i otvoriti u nekom podržanom okruženju(npr VS Code)
2. Pokretanje backend Node.js aplikacije
  2.1 Otvoriti novi terminal, uneti i izvršiti sledeće naredbe:
   cd Backend
   npm init
   npm install
   npm start
4. Kreirati online MongoDb bazu, izvršiti izmene za putanju ka sopstvenoj bazi u .env fajlu, kao i JSON fajlu za migracije
   3.1 Za izvršavanje migracija ka bazi otvoriti novi terminal, uneti i izvršiti sledeće naredbe:
     3.1.1 za izvrsavanje efekta migracije:
      migrate-mongo up
     3.1.2 za poništavanje efekta migracije (rollback):
     migrate-mongo down
  
5. Pokretanje frontend React aplikacije
   4.1 Otvoriti novi terminal, uneti i izvršiti sledeće naredbe:
   cd Frontend
   cd myapp
   npm install
   npm start
   
Kratak opis funkcionalnosti:
Aplikacija predstavlja primer društvene mreže. Korisnici mogu gledati sadržaj svojih prijatelja i ostavljati komentare ili reakcije na tom sadržaju. Svaki korisnik kreator ima svoj lični profil na kom takodje može podeliti svoja razmišljanja ili multimedijalni sadržaj. 
Korisnik radi sigurnosti, pre nego što postane član naše društvene mreže mora ostaviti svoje kredencijale i napraviti nalog, nakon čega uspešno može da se uloguje na našu aplikaciju. Pored samog sadržaja drugih korisnika, može se videti lista prijatelja, lista online korisnika, reklamni sadržaj, obaveštenja o rodjendanima,trentno vreme i vremenska prognoza..
Preko navigacionog meni bara lako se može preći sa početne na stranicu o profilu korisnika klikom na navigacione linkove, logo ili profilnu sliku. 
Naša aplikacija, ukratko, omogućava deljenje sadržaja i interakciju izmedju korisnika. Ona treba da obezbedi uloge: administratora, korisnika kreatora i korisnika posetioca.
Korisnik kreator ima uvid u listu prijatelja, može da pretražuje ostale korisnike, zapraćuje I odpraćuje ih. Ima mogućnost da postavlja I gleda sadržaj svojih prijatelja. Objavu može sadržati upload-ovanu fotografiju sa računara korisnika. Može da briše svoje objave, kao I da ostavlja reakcije.
Korisnici u ulozi administratora, pored nabrojanih mogućnosti imaju dozvolu I da brišu objave svih korisnika u eventualnom slučaju nedozvoljenog sadržaja.
Korisnici posetioci za razliku od korisnika kreatora nemaju mogućnost objavljivanja ličnog sadržaja. Oni imaju mogućnost ostavljanja reakcija, zapraćivanja, pretrage kao I gledanja sadžaja svojih prijatelja.


