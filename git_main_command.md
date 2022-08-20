# GIT MAIN COMMAND

# Prima COMMIT:
-echo "# multiple_view_2" >> README.md
-git init   # Inizializza la repositori locale
-git add README.md   # Aggiunge un file allo staging area
-git commit -m "first commit"   # Salva i dati nella repository locale
-git branch -M main   # Rinomina il branch corrente come main
-git remote add origin https://github.com/wiseright/multiple_view_2.git    # Crea un alias origin del link della repo remota
-git push -u origin main   # Salva i dati sulla repo remota origin

# Seconda COMMIT:
-git add README.md
-git commit -m "second_commit"
-git push -u origin main

# Creare una branca e fare il merge sulla main:
> Start a new feature
-git checkout -b new-feature main
> Edit some files
-git add <file>
-git commit -m "Start a feature"
> Edit some files
-git add <file>
-git commit -m "Finish a feature"
> Merge in the new-feature branch
-git checkout main
-git merge new-feature
-git branch -d new-feature


# Other command
-git branch   # Elenca tutte le branch locali
-git branch   -r   # Elenca tutte le branch remote
-git config user.email
-git config user.email <indirizzo_email>
-git log   # Ritorna la lista di tutte le commit
-git log --oneline   # Ritorna la lista di tutte le commit per ogni linea

# FEATCH command:
-git fetch origin    # Salva in locale (senza sovrascrivere) tutte le branch di origin 
-git fetch origin  new_branch  # Salva in locale (senza sovrascrivere) solo la branca new_branch

# CHECKOUT command:
-git checkout origin new_branch   # switcha alla branca