## Polityka Prywatności aplikacji Velo Sudoku

*Ostatnia aktualizacja: 20.03.2026*

> **Podsumowanie zmian (20.03.2026):**
> - Sekcja 2: Doprecyzowano, że dane partnerów są przesyłane wyłącznie po wyrażeniu zgody (nie automatycznie).
> - Sekcja 3B: Rozdzielono Firebase Analytics (Consent Mode v2 / TCF) od Crashlytics i Performance (osobna zgoda). Dodano informację o cookieless pings.
> - Sekcja 3C: Dodano Google Play Services (płatności).
> - Sekcja 5: Dodano możliwość usuwania pojedynczych wpisów w statystykach oraz zarządzanie zgodami w ustawieniach aplikacji.
> - Sekcja 6: Rozbudowano opis mechanizmów zgody: CMP (IAB TCF v2.2) dla reklam i analityki, osobny formularz dla raportów błędów i wydajności.

### 1. Wstęp
Niniejsza polityka prywatności określa zasady przetwarzania i ochrony danych w aplikacji mobilnej **Velo Sudoku** (dalej "Aplikacja"). Szanujemy prywatność użytkowników i dbamy o przejrzystość w kwestii wykorzystywanych technologii.

### 2. Dane, uprawnienia i brak backendu
Aplikacja nie posiada własnego serwera (backendu) i nie przesyła danych osobowych użytkownika do Dewelopera. Nie wymagamy zakładania konta, logowania się ani podawania imienia czy adresu e-mail.

Aplikacja przetwarza dane w następujący sposób:
* **Przetwarzanie lokalne:** Postępy w grze, ustawienia, czasy rozwiązywania łamigłówek oraz statystyki są zapisywane wyłącznie w bezpiecznej pamięci wewnętrznej urządzenia użytkownika.
* **Przetwarzanie przez partnerów:** Aplikacja korzysta z bibliotek zewnętrznych (SDK), które mogą gromadzić identyfikatory urządzenia oraz dane diagnostyczne, wyłącznie po uzyskaniu wyraźnej zgody Użytkownika. Żadne dane osobowe ani identyfikatory urządzenia nie są przesyłane do partnerów przed wyrażeniem tej zgody. Jedynym wyjątkiem są zanonimizowane, pozbawione identyfikatorów dane pomiarowe (tzw. cookieless pings), które Google Firebase może wysyłać w ramach mechanizmu Consent Mode v2 — szczegóły w sekcji 3B.

### 3. Partnerzy zewnętrzni i udostępnianie danych
Zintegrowaliśmy z Aplikacją usługi zaufanych podmiotów trzecich. Nie mamy bezpośredniego dostępu do danych gromadzonych przez te systemy.

**A. Google AdMob (Reklamy)**
Dostawca reklam. Może wykorzystywać identyfikatory urządzenia do personalizacji reklam.
* **Zgoda:** Reklamy spersonalizowane są wyświetlane tylko po wyrażeniu zgody w oknie CMP (Consent Management Platform) zgodnym ze standardem IAB TCF v2.2. Bez zgody reklamy mogą być wyświetlane w formie niespersonalizowanej.
* Polityka prywatności Google: https://policies.google.com/privacy

**B. Google Firebase (Analityka, Stabilność i Wydajność)**
Aplikacja korzysta z trzech usług Firebase, które podlegają **oddzielnym mechanizmom zgody**:

1. **Firebase Analytics (statystyki użytkowania):**
   * Zgoda na analitykę (`analytics_storage`) jest zarządzana przez CMP zgodny ze standardem IAB TCF v2.2 i mapowana na **TCF Purpose 1** ("Przechowywanie informacji na urządzeniu lub dostęp do nich").
   * Przy starcie aplikacji wszystkie sygnały Consent Mode v2 (analytics_storage, ad_storage, ad_user_data, ad_personalization) są domyślnie ustawiane na **DENIED**.
   * **Cookieless pings:** Nawet bez zgody użytkownika Google Firebase może wysyłać zanonimizowane dane pomiarowe pozbawione identyfikatorów urządzenia (tzw. cookieless pings) w ramach mechanizmu Consent Mode v2. Dane te nie zawierają informacji umożliwiających identyfikację użytkownika i służą wyłącznie do modelowania statystycznego.
   * Po wyrażeniu zgody w CMP sygnały są aktualizowane na GRANTED, co umożliwia pełne zbieranie danych analitycznych.

2. **Firebase Crashlytics (raporty o błędach) i Firebase Performance (dane o wydajności):**
   * Są zarządzane **osobnym mechanizmem zgody**, niezależnym od CMP i TCF.
   * Przy pierwszym uruchomieniu aplikacji wyświetlany jest formularz powitalny, w którym Użytkownik decyduje o włączeniu raportowania błędów i wydajności.
   * Bez wyrażenia tej zgody Crashlytics i Performance są całkowicie wyłączone — żadne raporty nie są wysyłane.
   * Użytkownik może zmienić tę decyzję w dowolnym momencie w Ustawieniach Aplikacji (sekcja "Prywatność").

* Polityka prywatności Firebase: https://firebase.google.com/support/privacy

**C. Google Play Services (Płatności)**
Aplikacja korzysta z usług Google Play do obsługi zakupów w aplikacji. Deweloper nie ma dostępu do danych finansowych Użytkownika.

### 4. Cel działań
Działania podejmowane przez Aplikację mają na celu:
1. **Funkcjonalność gry:** Zapisywanie stanu gry (Save/Load) – dane lokalne.
2. **Utrzymanie i rozwój:** Monitorowanie błędów i statystyk – tylko za zgodą Użytkownika.
3. **Monetyzacja:** Wyświetlanie reklam – spersonalizowane tylko za zgodą Użytkownika.

### 5. Usuwanie danych
Pełna kontrola nad danymi leży po stronie Użytkownika.

**Zarządzanie postępem gry (Dane Lokalne):**
* **Usuwanie pojedynczych wpisów:** Użytkownik ma możliwość ręcznego usunięcia wybranych wyników w sekcji Statystyk.
* **Całkowite usunięcie danych:** Aby trwale usunąć wszystkie postępy, należy odinstalować aplikację lub wyczyścić jej dane (*Ustawienia Androida -> Aplikacje -> Velo Sudoku -> Pamięć -> Wyczyść dane*).

**Zarządzanie zgodami (Dane Zewnętrzne):**
Użytkownik może w każdej chwili cofnąć lub zmienić swoje zgody w Ustawieniach Aplikacji (sekcja "Prywatność"):
* **Zgoda na reklamy i analitykę** — poprzez ponowne otwarcie formularza CMP.
* **Zgoda na raporty błędów i wydajności** — poprzez przełącznik w ustawieniach.
Cofnięcie zgody natychmiast zatrzyma przesyłanie odpowiednich danych do partnerów.

**Dane reklamowe (Google):**
Użytkownik może dodatkowo zresetować swój identyfikator reklamowy w ustawieniach urządzenia:
* *Ustawienia Androida -> Google -> Reklamy -> Zresetuj identyfikator reklamowy* lub *Usuń identyfikator reklamowy*.
* Aby zarządzać danymi powiązanymi z kontem Google, odwiedź: https://myactivity.google.com/

### 6. RODO / GDPR (Zgoda Użytkownika)
Zgodnie z RODO, użytkownicy z Europejskiego Obszaru Gospodarczego (EOG) i Wielkiej Brytanii mają pełne prawo decydowania o swoich danych.

Aplikacja stosuje **dwa oddzielne mechanizmy zbierania zgody:**

1. **Formularz CMP (Consent Management Platform):**
   * Wyświetlany przy pierwszym uruchomieniu aplikacji, zgodny ze standardem **IAB TCF v2.2**.
   * Użytkownik decyduje w nim o zgodzie na **reklamy spersonalizowane** oraz **analitykę** (TCF Purpose 1).
   * Zgody na reklamy (`ad_storage`, `ad_user_data`, `ad_personalization`) i analitykę (`analytics_storage`) są od siebie **niezależne** — użytkownik może zaakceptować jedno bez drugiego.
   * Formularz CMP można ponownie otworzyć w Ustawieniach Aplikacji (sekcja "Prywatność").

2. **Formularz powitalny (Raporty błędów i wydajności):**
   * Wyświetlany przy pierwszym uruchomieniu, osobno od CMP.
   * Użytkownik decyduje o włączeniu **Firebase Crashlytics** (raporty o błędach) i **Firebase Performance** (dane o wydajności).
   * Decyzję można zmienić w dowolnym momencie w Ustawieniach Aplikacji.

Jeśli Użytkownik nie wyrazi zgody:
* Żadne dane osobowe ani identyfikatory urządzenia nie zostaną wysłane do Google Firebase ani AdMob.
* Google Firebase może jedynie wysyłać zanonimizowane cookieless pings w ramach Consent Mode v2, które nie zawierają danych umożliwiających identyfikację użytkownika.

### 7. Kontakt
W sprawach dotyczących polityki prywatności prosimy o kontakt pod adresem e-mail:
**minigamesforeveryone@gmail.com**

*Wskazówka: Aby przyspieszyć odpowiedź w kwestiach związanych z RODO/Prywatnością, prosimy o wpisanie w tytule wiadomości słowa "Prywatność" lub "RODO".*
