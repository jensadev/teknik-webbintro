# Introduktion till webbutveckling

För att komma igång och jobba med webben kommer vi även att arbeta med lite olika verktyg. Tanken med det är att du ska få se och prova på verktyg som du kommer att arbeta med de kommande åren här på teknikprogrammet. Verktygen är utvalda för att de är relevanta för din eventuellt kommande yrkesroll.

Programmen behövs för att du ska kunna
* skriva kod och få hjälp i processen, IDE, [Visual Studio Code](https://code.visualstudio.com/)
* versionshantera sidan, [Git](https://git-scm.com/)
* hosta sidan, [GitHub](https://www.github.com/)
* navigera i filsystemet på din dator med terminalen

Du kommer att behöva registrera ett konto på https://github.com/

## Visual Studio Code

Visual Studio Code är ett så kallat IDE, Integrated Development Environment, vilket är ett program som är anpassat för att skriva kod. Det finns många olika IDEs och de är anpassade för olika språk och miljöer. Visual Studio Code är ett väldigt populärt IDE som är gratis och som fungerar för många olika språk och miljöer.

### Installation

Det kan vara så att du redan har Visual Studio Code installerat på din dator, testa genom att öppna start-menyn och söka efter “vscode". Om du inte har det så kan du ladda ner det från https://code.visualstudio.com/ och installera det.

### Test

* Vad är Visual Studio Code för typ av program?
* Vilket företag ligger bakom Visual Studio Code?

## GIT

Git är ett så kallat versionshanteringssystem, det är ett sätt för de som arbetar med kod att samarbeta, hantara och spåra ändringar i koden. Det är ett väldigt kraftfullt verktyg som används av de flesta utvecklare idag.

Tillsammans med Git så använder vi oss av GitHub som är en tjänst för att lagra och dela med sig av kod.

### Installation

För att installera Git så går du till https://git-scm.com/ och laddar ner programmet. När du installerar så kan du välja att använda Git Bash som terminal, det är en terminal som är anpassad för att användas med Git.

Ladda ned programmet och starta installationen (om den ställer massa frågor så svara enligt nedan).

1. Du behöver inte byta installations-plats för Git.
2. Du behöver inte ändra installations-egenskaperna.
3. För editor så välj Visual Studio Code.
4. För branch, välj “Override” och “main”. Detta är en nyare standard för GitHub.
5. För PATH, så välj “Git from the command line and also from 3rd-party software”.
6. Du behöver inte ändra något för SSL och HTTPS.
7. Du behöver inte ändra på line endings.
8. Viktigt För terminal emulator så välj att använda MinTTY.
9. Du behöver inte ändra “default behaviour of git pull”.
10. Viktigt Välj att installera Git Credential Manager (du behöver den senare när du använder GitHub).
11. Du behöver inte ändra “extra options” eller “experminental options”.

### Test

* Vad är Git för något?
* Ge minst två exempel på användningsområden för Git.

## GitHub

GitHub är en tjänst för att lagra och dela med sig av kod. Det är en tjänst som är väldigt populär och används av många företag och organisationer. På Git sparas kod i det som kallas för ett repository, vilket är en mapp som innehåller all kod för ett projekt. Du läser just nu en README-fil som finns i ett repository på GitHub.

### Registrering

För att kunna använda GitHub så behöver du registrera ett konto på https://github.com/ och sedan logga in.

### Skapa ett repository på GitHub

När du har registrerat dig och loggat in så kan du skapa ett repository genom att klicka på “New” i övre högra hörnet. Då kommer du till en sida där du kan skapa ett nytt repository. Fyll i ett namn (till exempel teknik-webb) på ditt repository och klicka på “Create repository”.

### Ladda ned ett repository från GitHub

**Innan du gör detta så är det viktigt att du navigerar till rätt mapp i terminalen.**

Öppna ```Git Bash``` och skriv följande kommando:

```bash
pwd
```

Detta kommer att visa vilken mapp du är i. Om du inte är i rätt mapp (```/c/code```)så kan du navigera till rätt mapp genom att skriva följande kommando (där ```<mapp>``` är namnet på mappen du vill navigera till):

```bash
cd <mapp>
```

Mappen du ska navigera till är ```/c```, det är roten i ditt filsystem i Windows.

I ```/c``` så ska du skapa en ny mapp som heter ```code```. Det gör du genom att skriva följande kommando:

```bash
mkdir code
```

Nu ska du navigera till mappen ```code```. Det gör du genom att skriva följande kommando:

```bash
cd code
```

Dubbekolla att du är i rätt mapp genom att skriva följande kommando:

```bash
pwd
```

Det ska då stå ```/c/code```.

**Snyggt jobbat, nu är du i rätt mapp och kan ladda ned ett repository.**

För att ladda ned ett repository så behöver du först kopiera länken till det. Det gör du genom att klicka på den gröna knappen “Code” och sedan kopiera länken som visas. Öppna sedan Git Bash och skriv följande kommando:

```bash
git clone <länk>
```

Git kommer då att ladda ned repositoryt till din dator och skapa en mapp med samma namn som repositoryt.

Bra jobbat, nu har du laddat ned ett repository till din dator och kan börja arbeta med det.

Byt mapp till det repository du laddade ned genom att skriva följande kommando:

```bash
cd <repository>
```

Du kan nu öppna Visual Studio Code genom att skriva följande kommando:

```bash
code .
```

### Test

* Vad är GitHub för något?
* Vad är ett repository?

* Ge minst två exempel på bash kommandon som du har använt.

## Webbsida

Nu ska vi äntligen komma igång med att skapa en webbsida. Vi kommer att använda oss av HTML, CSS. Vi kommer att använda oss av Visual Studio Code för att skriva koden och vi kommer att använda oss av Git för att versionshantera koden och GitHub för att lagra koden.

HTML är ett språk som används för att skapa webbsidor. Det är ett språk som används för att strukturera upp en webbsida. Tillsammans med HTML så använder vi oss av CSS som är ett språk som används för att styla en webbsida.

### Förberedelser

Se till att du är i mappen du har skapat för ditt repository. Om du inte är det så kan du navigera till rätt mapp genom att skriva följande kommando (där ```<mapp>``` är namnet på mappen du vill navigera till). Om du har följt instruktionerna ovan så ska du vara i mappen ```/c/code/<repository>```.

```bash
cd <mapp>
```

Öppna sedan mappen i Visual Studio Code genom att skriva följande kommando:

```bash
code .
```

### Skapa en webbsida

Nu ska vi skapa en webbsida. Vi kommer att skapa en webbsida som heter index.html. Det är en standard som används för att skapa en startsida för en webbsida. Vi kommer att skapa en webbsida som innehåller en rubrik och en paragraf.

Skapa en ny fil som heter index.html genom att klicka på “File” och sedan “New File”. Döp filen till index.html genom att klicka på “File” och sedan “Save As”. Skriv in namnet på filen och klicka på “Save”.

**När en webbserver läser en webbsida så läser den alltid först en fil som heter index.html. Det är därför vi döper filen till index.html.**

Skriv nu följande i filen, ```html:5``` tryck sedan på tabb-tangenten. Det kommer att skapa en mall för en webbsida. Krånglar det, ta bort och skriv igen.

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>
  
</body>
</html>
```

Detta är grundstrukturen för en webbsida skriven i HTML. Först så anges vilken typ av dokument det är. Detta följs av ```html``` taggen som innehåller all HTML-kod. I ```html``` taggen så finns det två taggar, ```head``` och ```body```. I ```head``` taggen så finns det information om webbsidan som inte syns på webbsidan. I ```body``` taggen så finns all HTML-kod som syns på webbsidan.

Vi ska nu lägga till en rubrik och en paragraf i ```body``` taggen. Det gör vi genom att använd en rubrik-tagg, ```h1```, och en paragraf-tagg, ```p```. Det gör vi genom att skriva följande i ```body``` taggen.

```html
<h1>Min webbsida</h1>
<p>Detta är min första webbsida</p>
```

Spara sedan filen. Du ska nu använda en extension som heter Live Server för att ladda sidan i din webbläsare.

### Live Server

Klicka på “Extensions” (```CTRL+SHIFT+x```) eller hitta det i "View" menyn i Visual Studio Code. I extensions söker du efter Live Server. Installera extensionen och följ instruktionerna för att aktivera den.

När du har aktiverat Live Server så kan du klicka på “Go Live” i nedre högra hörnet. Det kommer att öppna en webbläsare och ladda sidan. Du kan nu se hur din webbsida ser ut.

### Test

* Vad är HTML för något?
* Vad är CSS för något?


### Versionshantering

Nu ska du använda Git för att versionshantera din kod. Du kommer att göra det med hjälp av Visual Studio Code.

För att versionshantera din kod så behöver du först lägga till filerna i ett så kallat staging area. Det gör du genom att klicka på “Source Control” (```CTRL+SHIFT+G```) eller hitta det i "View" menyn i Visual Studio Code. Klicka sedan på “+” för att lägga till filerna i staging area.

När du har lagt till filerna i staging area så behöver du skriva en commit message. Det är ett meddelande som beskriver vad du har gjort. Meddelandet skriver du i fältet “Message” och sedan klickar du på "Commit" knappen.

När en comm

## CSS

## En bild

**Ett viktigt tips när du arbetar med filer för webben och GitHub är att du inte ska använda mellanslag i filnamn. Istället så ska du använda dig av bindestreck. Undvik även stora bokstäver och specialtecken.**