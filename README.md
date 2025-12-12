# podstawy-ukw-miki

Git Cheat Sheet – Podstawy


🔧 Konfiguracja

git config --global user.name "Twoje Imię"
git config --global user.email "twoj@email.com"
git config --list     # pokazuje konfigurację

📁 Inicjalizacja repozytorium

git init              # tworzy nowe repo w bieżącym katalogu
git clone <url>       # klonuje istniejące repo

📊Status, logi, różnice

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

☁️ Push & Pull

git remote -v                # lista zdalnych repo
git push origin <gałąź>      # wysyła zmiany
git pull                     # pobiera i scala
git fetch                    # pobiera, ale NIE scala

♻️ Wycofywanie i resetowanie

git restore <plik>           # przywraca plik z commitów
git restore --staged <plik>  # usuwa plik ze stage
git reset HEAD~1             # usuwa ostatni commit (lokalnie)
git reset --hard <commit>    # reset do wskazanego commita (uwaga!)
git revert <commit>          # tworzy commit cofający

🔍 Stash – odkładanie zmian

git stash            # odkłada bieżące zmiany
git stash list       # lista stashy
git stash apply      # przywraca zmiany
git stash pop        # przywraca i usuwa stash

🗑️ Usuwanie plików

git rm <plik>        # usuwa plik i staged
git rm --cached <plik> # usuwa z git, zostawia na dysku

🧪 Tagi

git tag              # lista tagów
git tag <nazwa>      # tworzy tag
git push --tags      # wysyła tagi