# Strona Internetowa TanieDanie (Wizytówka + Strony Prawne)

Oficjalny, nowoczesny i responsywny serwis internetowy dla aplikacji mobilnej **TanieDanie** (Zero-Waste & Promocje AI).

Projekt przygotowany w standardzie **HTML5 + Tailwind CSS**, bez skomplikowanych zależności — ładuje się błyskawicznie (100/100 na Google PageSpeed) i jest w 100% gotowy do darmowego wdrożenia w chmurze (Vercel, Cloudflare Pages, Netlify, GitHub Pages).

---

## 📁 Struktura plików

* **`index.html`** — Główna strona (Landing Page):
  * Prezentacja aplikacji, hasła przewodnie, korzyści (oszczędność do 300 zł/mies.).
  * Interaktywny podgląd ekranu aplikacji (mockup telefonu).
  * Kluczowe moduły: Promocje z dyskontów, AI Zero-Waste, Meal Prep, Złote Przepisy, Inteligentny koszyk.
  * Przewodnik „Jak to działa w 3 krokach”.
  * Interaktywny akordeon z najczęstszymi pytaniami (FAQ).
  * Oficjalne przyciski pobrania z Google Play.
* **`terms.html`** — Regulamin Serwisu i Aplikacji:
  * Zawiera kluczową **klauzulę AI Disclaimer** (charakter inspiracyjny, weryfikacja alergenów i zdatności produktów przez użytkownika).
  * Zastrzeżenie cenowe (ceny z gazetek jako informacja, nie oferta handlowa w myśl Kodeksu Cywilnego).
  * Informacja o niezależności od znaków towarowych Biedronki, Lidla itp.
* **`privacy.html`** — Polityka Prywatności i RODO:
  * Wymagana przez Google Play i prawo unijne (RODO/GDPR).
  * Precyzyjnie opisuje dane (e-mail, zahashowane hasło bcrypt, preferencje).
  * Wymienia procesorów (Microsoft Azure OpenAI, Google Firebase FCM, Pexels API).
  * Prawa użytkownika (dostęp, usunięcie, sprostowanie).
* **`delete-account.html`** — Procedura Usuwania Konta i Danych:
  * **Obowiązkowy wymóg Google Play Developer** (Data Deletion Policy URL).
  * Instrukcja usunięcia bezpośrednio z aplikacji (*Profil -> Usuń konto*).
  * Formularz zgłoszeniowy i kontakt e-mail dla osób, które odinstalowały aplikację.
* **`contact.html`** — Strona kontaktowa ze wsparciem i formularzem.
* **`vercel.json`** & **`netlify.toml`** — Gotowe konfiguracje dla czystych adresów URL (np. `/privacy` zamiast `/privacy.html`).

---

## 🚀 Jak podejrzeć stronę lokalnie?

Strona działa od razu — możesz po prostu kliknąć dwukrotnie w plik `index.html` w eksploratorze Windows, aby otworzyć ją w przeglądarce.

Możesz też uruchomić lokalny serwer HTTP:
```bash
npm start
```
I otworzyć w przeglądarce adres: `http://localhost:3000`.

---

## 🌐 Jak wrzucić stronę do Internetu za darmo? (W 2 minuty)

### Opcja 1: Vercel (Najwygodniejsza)
1. Zainstaluj CLI Vercela lub wejdź na [vercel.com](https://vercel.com).
2. W terminalu w tym folderze wpisz:
   ```bash
   npx vercel
   ```
3. Postępuj zgodnie z instrukcjami na ekranie (zaloguj się przez GitHub/Google).
4. Otrzymasz natychmiast darmowy adres HTTPS (np. `taniedanie.vercel.app`), z którego możesz podpiąć własną domenę.

### Opcja 2: Cloudflare Pages
1. Zaloguj się na [dash.cloudflare.com](https://dash.cloudflare.com) -> Workers & Pages.
2. Wybierz *Create Application* -> *Pages* -> *Direct Upload*.
3. Przeciągnij i upuść ten folder `C:\taniedanie-website`.
4. Gotowe! Strona działa na nielimitowanym, darmowym hostingu Cloudflare.

---

## 📱 Jakie linki wkleić w Google Play Console?

Po wdrożeniu strony wklej odpowiednie adresy w panelu **Google Play Console** (w zakładce *Zawartość aplikacji*):
1. **Polityka prywatności (Privacy Policy URL)**:
   `https://twoja-domena.pl/privacy`
2. **Usuwanie konta i danych (Data Deletion URL)**:
   `https://twoja-domena.pl/delete-account`
