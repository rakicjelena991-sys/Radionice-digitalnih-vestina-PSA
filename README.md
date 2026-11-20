PSA — RADIONICE DIGITALNIH VEŠTINA

Projekat je namenjen za Visual Studio 2022 na Windows računaru.
Potrebni su ASP.NET and web development workload i .NET Framework 4.7.2 targeting pack.

1. Raspakujte ceo ZIP.
2. Otvorite PSARadionice.sln u Visual Studio-u.
3. U slučaju nedostajućih referenci, izaberite Restore NuGet Packages ili u Package Manager Console pokrenite Update-Package -reinstall.
4. Ako Visual Studio traži IIS Express konfiguraciju, dozvolite da je kreira.
5. Pokrenite F5 / IIS Express i otvorite početnu stranicu.
6. Proverite meni, prikaz radionica, prijavu sa praznim/neispravnim podacima i potvrdu validne prijave.

Napomene o validaciji:
- Sva pravila validacije proveravaju se na serveru (ClientValidationEnabled = false u Web.config, jer projekat nema jQuery validation skripte).
- Polje Email ima type="email", pa browser sam zaustavi slanje ako je format očigledno pogrešan (npr. "test").
- Za prikaz serverskih poruka: pošaljite praznu formu ili unesite ime od dva slova.

Aplikacija ne koristi bazu podataka. Poslati podaci se proveravaju i prikazuju samo u odgovoru (potvrdi), bez trajnog čuvanja i bez slanja emaila.

