# Gwiazdozbiór Orion - laboratorium git

Repozytorium zawiera stronę internetową poświęconą gwiazdozbiorowi Orion wraz z ćwiczeniami z obsługi systemu git.

![Mgławica Orion](src/nasa_01.png)  
Źródło: [NASA/JPL-Caltech/UCLA](https://www.nasa.gov)

## Lista wykonanych zadań

- [x] Główny plik HTML (`index.html`)
- [x] Plik licencji (`LICENSE.md`) - uzupełniony o imię, nazwisko i rok 2025
- [x] Kod CSS (`style.css`)
- [x] Edycja wyświetlania znaczników (rozbudowane style dla nav, footer, body, tabela, obrazy)
- [x] Dodanie dwóch podstron HTML (`pages/about.html`, `pages/links.html`)
- [x] Plik markdown jako opis/manuał projektu (ten plik)

## Przebieg pracy - kolejno tworzone gałęzie i zmiany

### 1. Gałąź `Galaz-1` / `feature-html`

- Utworzono plik `index.html` z pełną strukturą HTML5
- Dodano nagłówki, nawigację, sekcje artykułów, tabelę z gwiazdami, zdjęcie w `<figure>`
- Poprawiono język dokumentu na `lang="pl"` oraz link do PG w `<nav>`
- Zapisano zmiany w `readme.md` o utworzeniu pliku HTML
- Wykonano commit i merge do `main`

### 2. Gałąź `Galaz-css` / `feature-css`

- Rozbudowano plik `style.css`
- Dodano ciemne tło kosmiczne dla całego dokumentu (`body`)
- Ustawiono tło oraz minimalną wysokość i szerokość dla elementów `<nav>` i `<footer>`
- Dodano stylowanie nagłówków, tabeli, obrazów i efektów hover
- Zapisano w `readme.md` informację o zmianach w stylach
- Wykonano merge do `main`

### 3. Gałąź `Galaz-info` / `feature-amend`

- Utworzono plik `info.txt` z aktualną pogodą (20.11.2025 Gdańsk)
- Początkowo wykonano commit tylko z tym plikiem
- Następnie użyto `git commit --amend`, aby dołączyć zapomniane pliki do tego samego commita
- W logach widoczna jest tylko jedna, poprawiona wersja commita
- Opisano tę operację w `readme.md`
- Wykonano merge do `main`

### 4. Gałąź `Galaz-markdown`

- Znacząco rozbudowano ten plik `readme.md`
- Dodano nagłówki drugiego poziomu (`##`), linki, checkboxy `[x]`, opis wszystkich gałęzi
- Zamiast zwykłego merge wykonano `git rebase main`
- Opisano efekt rebase (historia liniowa, brak merge commitów)

### 5. Gałąź `html-subpage` - Lab 4, zadanie 3.2 (04.12.2025)

- Utworzono folder `pages` oraz dwie podstrony: `about.html` i `links.html`
- Podstrona „O mnie” zawiera opis zainteresowań, planów zawodowych i studiów
- Podstrona „Źródła” zawiera listę linków wykorzystanych w projekcie (NASA, Wikipedia, Markdown Guide itp.)
- Dodano linki do podstron w nawigacji głównej (`index.html`)
- Wykonano commit i wypchnięto gałąź na zdalne repozytorium GitHub

### Decyzja o sposobie scalania (Lab 4, zadanie 3.2 - 04.12.2025)

Po zakończeniu prac na gałęzi `html-subpage` wykonałem scalanie z `main` przy użyciu polecenia:  
`git rebase html-subpage` (będąc na gałęzi main).

### 6. Gałąź `main` - stan ostateczny (04.12.2025)

- Uzupełniono plik `LICENSE.md` o dane autora i rok 2025
- Wszystkie zmiany zostały scalone, repozytorium jest czyste
- Wygenerowano końcowe logi:  
  `git log --graph --all --decorate --oneline > log_final.txt`

## Źródła

- [NASA - zdjęcie Mgławicy Orion](https://www.nasa.gov)
- [Markdown Guide - podstawy składni](https://www.markdownguide.org/basic-syntax/)
- [Dokumentacja Git](https://git-scm.com/doc)
- [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)
- [W3Schools - HTML/CSS](https://www.w3schools.com)

---

**Danila Minkou**  
Indeks: **211365**  
Laboratorium NITiJP - semestr zimowy 2025/2026  
Data aktualizacji: **04.12.2025**
