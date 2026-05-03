# Justyna Wankiewicz

Statyczna strona portfolio/CV przygotowana do publikacji na GitHubie i Vercel.

## Pliki

- `index.html` - struktura strony i treści
- `styles.css` - wygląd, responsywność i doodle-akcenty
- `script.js` - menu mobilne i aktualny rok w stopce

## Uruchomienie lokalne

Możesz otworzyć `index.html` bezpośrednio w przeglądarce albo uruchomić prosty lokalny serwer:

```bash
python3 -m http.server 5173
```

Po uruchomieniu serwera strona będzie dostępna pod adresem:

```text
http://localhost:5173
```

## Publikacja na Vercel

1. Utwórz repozytorium na GitHubie.
2. Wrzuć do niego pliki z tego folderu.
3. W Vercel wybierz `Add New Project`.
4. Podłącz repozytorium.
5. Dla statycznej strony nie trzeba ustawiać komendy build.

## Następne kroki

- Uzupełnić konkretne projekty portfolio.
- Dodać link do LinkedIn lub CV PDF, jeśli ma być dostępne do pobrania.
- Opcjonalnie przygotować wersję angielską.


## Edycja strony

Najczęściej edytowane miejsca:

- Treści sekcji: zmieniaj teksty w `index.html`.
- Kolory: główna paleta jest na początku `styles.css` w selektorze `:root`. Aktualnie bazuje na trzech akcentach: niebieskim, limonkowym i fioletowym.
- Favicon i znak marki: edytuj `favicon.svg` oraz element `.brand-mark` w `index.html`.
- Układ i odstępy: edytuj klasy sekcji w `styles.css`, np. `.hero`, `.skills-grid`, `.portfolio-grid`.
- Kontakt: podmień adresy `mailto:` w `index.html`.

Po każdej zmianie odśwież stronę w przeglądarce. Jeśli używasz lokalnego serwera, nie musisz go restartować przy zmianach HTML/CSS/JS.

## Wdrożenie zmian na GitHub

Po zapisaniu zmian uruchom w folderze projektu:

```bash
git status
git add .
git commit -m "Update visual design"
git push
```

Jeśli lokalny folder nie jest jeszcze repozytorium Git, uruchom najpierw jednorazowo:

```bash
git init
git add .
git commit -m "Initial personal website"
git branch -M main
git remote add origin ADRES_TWOJEGO_REPOZYTORIUM
git push -u origin main
```

Jeśli repozytorium jest podpięte do Vercel, Vercel automatycznie wykryje nowy commit i wdroży aktualną wersję strony.
