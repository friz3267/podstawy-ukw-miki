# podstawy-ukw-miki

Git Cheat Sheet – Podstawy
🔧 Konfiguracja
git config --global user.name "Twoje Imię"
git config --global user.email "twoj@email.com"
git config --list     # pokazuje konfigurację

📁 Inicjalizacja repozytorium
git init              # tworzy nowe repo w bieżącym katalogu
git clone <url>       # klonuje istniejące repo

Status, logi, różnice
git status            # status zmian
git log               # historia commitów
git log --oneline     # skrócony log
git diff              # porównanie zmian

➕ Dodawanie i zatwierdzanie zmian
git add <plik>        # dodaj plik do stage
git add .             # dodaj wszystkie zmiany
git commit -m "opis"  # commit ze zmianami
git commit -am "opis" # add + commit (tylko zmodyfikowane pliki)

🌿 Praca z gałęziami (branches)
git branch            # lista gałęzi
git branch <nazwa>    # tworzy gałąź
git checkout <gałąź>  # przejście na gałąź
git switch <gałąź>    # nowsza wersja przełączania
git switch -c <nowa>  # tworzy i przełącza
git merge <gałąź>     # łączy gałąź z obecną