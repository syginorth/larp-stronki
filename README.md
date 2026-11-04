# larp-stronki

Zbiór jednoplikowych stron do portfolio.

## `soda/` — Syk, napój gazowany zero cukru

Pełnoekranowy landing page koncepcyjnej (fikcyjnej) marki napoju. Jeden plik `index.html`,
bez kroku budowania — wystarczy otworzyć go w przeglądarce albo wystawić na GitHub Pages.

**Co się dzieje na stronie**

- Ekran ładowania z puszką, która „napełnia się” w rytm wczytywania modelu 3D.
- Puszka 3D (`<model-viewer>`) wychyla się za kursorem; można ją obrócić, przeciągając myszą lub palcem.
- Wiśnie i jagody 3D unoszą się z paralaksą i uciekają przed kursorem.
- Zmiana smaku (karty, strzałki albo ← / → na klawiaturze): tło i kolor akcentu płynnie się zmieniają,
  puszka robi obrót 720° z rozmyciem i zmienia etykietę, owoce zapadają się do środka i wybuchają
  w nowe miejsca, a wielki napis w tle („WIŚNIA” / „JAGODA”) wymienia litery.
- „Kup teraz” dodaje do koszyka (licznik + powiadomienie + chmurka bąbelków).
- Widok mobilny z menu rozwijanym, obsługa dotyku i `prefers-reduced-motion`.

**Technologie:** HTML, CSS, JavaScript, [GSAP 3](https://gsap.com/),
[Google model-viewer](https://modelviewer.dev/). Czcionki: Lobster, Inter, Manrope, Outfit (Google Fonts).

Modele 3D i grafiki są wczytywane z zewnętrznego serwera (`ASSET_BASE_URL` w skrypcie).
