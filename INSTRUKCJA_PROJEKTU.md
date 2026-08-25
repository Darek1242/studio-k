# Instrukcja Obsługi i Zarządzania Stroną

## 1. Struktura Projektu

- `src/pages/index.astro`: Główna treść strony.
- `src/layouts/Layout.astro`: Główny szablon.
- `src/styles/global.css`: Definicje kolorów i globalnych stylów.
- `src/content/portfolio/`: Wpisy do portfolio (Markdown).
- `src/data/blocked-dates.json`: Zajęte terminy.

## 2. Jak wprowadzać zmiany?

- **Tekst i Układ:** Edytuj plik `src/pages/index.astro`.
- **Kolorystyka:** Edytuj `src/styles/global.css`.
- **Portfolio:** Dodaj pliki `.md` do `src/content/portfolio/`.

## 3. Komendy Publikacji (Workflow)

Po każdej zmianie w kodzie wykonuj następujący cykl:

```bash
# Pobierz najnowsze zmiany z repozytorium
git pull --rebase origin main

# Dodaj zmiany i wyślij na serwer
git add .
git commit -m "Krótki opis zmiany"
git push origin main
```

## 4. Lokalne testowanie

Przed publikacją zawsze sprawdź stronę lokalnie:

```bash
npm run dev
```
