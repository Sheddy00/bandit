# Level 0 -> level 1
## commande 
```ssh
cat readme
```

> password : NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL 

# Level 1 -> level 2
## commande 
```ssh
cat ./-
```

> password : rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi

# Level 2 -> level 3
## commande 
```ssh
cat ‘./spaces in this filename’
```

> password : aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG

# Level 3 -> level 4
## commande 
```ssh
find inhere
cd inhere
cat ./.hidden
```

> password : 2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe

# Level 4 -> level 5
## commande 
```ssh
ls
cd inhere/
find
file ./*
cat ./-file07
```

> password : lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR

# Level 5 -> level 6
## commande 
```ssh
ls
cd inhere/
find -type f -size 1033c ! -executable -exec file {} + | grep ‘ASCII text’ | cut -d ‘ :’ -f 1 | xargs cat 
```

> password : P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU

# Level 6 -> level 7
## commande 
```ssh
find
find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null
cat /var/lib/dpkg/info/bandit7.password
```

> password : z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S

# Level 7 -> level 8
## commande 
```ssh
ls
grep "millionth" data.txt | cut -d " " -f 2
```

> password : TESKZC0XvTetK0S9xNwm25STk5iWrBvP

# Level 8 -> level 9
## commande 
```ssh
ls
sort data.txt | uniq -u | grep -oE "[0-9a-zA-Z]{32}"
```

> password : EN632PlfYiZbn3PhVK3XOGSlNInNE00t

# Level 9 -> level 10
## commande 
```ssh
strings data.txt | grep "^==*" | grep -o "[[:print:]]*"
```

> password : G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s
# Level 10 -> level 11
## commande 
```ssh
base64 -d data.txt
```

> password : 6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM

# Level 11 -> level 12
## commande 
```ssh
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```

> password : JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv

# Level 12 -> level 13
## commande 
```ssh
mkdir /tmp/shedds
cp ~/data.txt /tmp/shedds/
cd /tmp/shedds
xxd -r data.txt data
```

> password :