# git-help
Lite småinstruktioner hur jag brukar göra med git

## Skapa ett nytt repo
Det finns olika vägar du kan gå för att ha ett repo på Github. Jag kommer att gå igenom två vis.

### Du skapar först ett repo med en readme.md-fil på Github
1. Skapa ett repo på Github, se till att bocka i att det ska med en readme-fil
2. Nu finns det en grön knapp där det står "code" till höger, tryck på den
3. Kopiera adressen som står där, den länkar till ditt repo
4. Gå till valfri terminal/kommandotolk på din dator och navigera till den mapp du vill lägga in ditt projekt i
5. använd ```cd ..``` för att steppa upp i mapphierarkin eller ```cd mappnamn``` för att steppa in i en undermapp
6. När du befinner dig där du vill ha ditt nya projekt i din terminal skriver du ```git clone länkenDuKopieratFrånGithub```
7. Tryck enter
8. Klar! Nu ska du ha ditt projekt lokalt och det ska vara länkat till din Github så du kan commita din grymma kod i tid och otid.

### Du skapar ett projekt lokalt på din dator och vill koppla den till ditt repo på Github
1. Du har redan en mapp för ditt projekt på din dator med minst en fil med något innehåll i
2. Du har ett helt tomt repo på din Github, ingen readme-fil
3. Kopiera länken till ditt repo på Github. ```https://github.com/användarnamn/reponamn.git```
4. Gå till valfri terminal/kommandotolk på din dator och navigera till den mapp där du har ditt projekt i
5. Skriv ```git init``` för att initiera ett nytt git-repo lokalt på din dator. Sen enter.
6. Skriv ```git add .``` för att alla dina filer i din mapp ska kunna hänga med i din commit sen. Sen enter.
7. Skriv ```git commit -m "ditt commitmeddelande"``` för att ge din commit ett bra namn. Sen enter.
8. Skriv ```git branch -M main``` för att döpa din branch till 'main'. Sen enter.
9. Skriv ```git remote add origin https://github.com/användarnamn/reponamn.git```. Sen enter.
10. Skriv ```git push -u origin main```. Sen enter.
11. Klar! Nu ska du se dina lokala filer som du pushat upp på Github!

## Pusha upp ny kod du har lokalt till ditt repo Github
1. ```git add .```
2. ```git commit -m "namn på din commit"```
3. ```git push```
4. Klar! Nu ska du se din nya grymma kod uppe på Gittan.
