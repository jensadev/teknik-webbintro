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

Det kan vara så att du redan har Git installerat på din dator, testa genom att öppna start-menyn och söka efter git". Det du ska hitta är "Git Bash". Om du inte har det så kan du ladda ner det från https://git-scm.com/ och installera det.

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

Spara sedan filen. Du ska nu använda en extension som heter Live Server för att 
ladda sidan i din webbläsare.

### Live Server

Klicka på “Extensions” (```CTRL+SHIFT+x```) eller hitta det i "View" menyn i Visual Studio Code. I extensions söker du efter Live Server. Installera extensionen och följ instruktionerna för att aktivera den.

När du har aktiverat Live Server så kan du klicka på “Go Live” i nedre högra hörnet. Det kommer att öppna en webbläsare och ladda sidan. Du kan nu se hur din webbsida ser ut.

### Test

* Vad är HTML för något?
* Varför döper vi filen till index.html?
* Vad är en tagg?

### Versionshantering

Nu ska du använda Git för att versionshantera din kod. Du kommer att göra det med hjälp av Visual Studio Code.

**Innan du kan göra commits så måste du berätta för Git vem du är.**

Öppna Git Bash och skriv följande kommandon:

```bash
git config --global user.name "DITT NAMN ELLER ANVÄNDARNAMN PÅ GITHUB"
git config --global user.email "DIN E-POSTADRESS SOM DU ANVÄNDE PÅ GITHUB"
```

**Det kan även vara så att VSCode kommer starta Git credentials manager (popup/webbläsarlogin) och be dig logga in på GitHub. Detta är för att autentisera VSCode så att du kan använda Git med det.**

För att versionshantera din kod så behöver du först lägga till filerna i ett så kallat staging area. Det gör du genom att klicka på “Source Control” (```CTRL+SHIFT+G```) eller hitta det i "View" menyn i Visual Studio Code. Klicka sedan på “+” för att lägga till filerna i staging area.

När du har lagt till filerna i staging area så behöver du skriva en commit message. Det är ett meddelande som beskriver vad du har gjort. Meddelandet skriver du i fältet “Message” och sedan klickar du på "Commit" knappen.

När en commit är gjord så behöver du skicka upp den till GitHub. Det gör du genom att klicka på "Sync Changes" knappen (som bör synas istället för "Commit" knappen).

När du väl pushat din kod till GitHub kan du öppna repositoryt på GitHub och se att din kod finns där.

**Tänk på att du är ansvarig för allt material du laddar upp och har på GitHub. Det är inte tillåtet att ladda upp material som du inte har rättigheter till.**

## En bild

För att göra sidan lite mer visuellt intressant ska vi nu lägga till en bild. Det kan vara en bild som du har tagit själv eller en bild som du har hittat på nätet. Det är viktigt att du har rättigheter till bilden och får använda den.

Först behöver du spara bilden så att Visual Studio Code kan hitta den. Om du vill kan du skapa en ny mapp i projektet, döpa den till ```img``` och spara bilden där. Du kan också spara bilden i samma mapp som index.html. För att spara bilden är den enklast att dra den från utforskaren i Windows till Visual Studio Code.

**Ett viktigt tips när du arbetar med filer för webben och GitHub är att du inte ska använda mellanslag i filnamn. Istället så ska du använda dig av bindestreck. Undvik även stora bokstäver och specialtecken.**

När du har sparat bilden så behöver du lägga till den i din webbsida. Det gör du genom att använda en ```img``` tagg. Det gör du genom att skriva följande i ```body``` taggen.

```html
<img src="img/bild.jpg" alt="En bild">
```

### Bildstorlek

Det är viktigt att tänka på bildstorleken när du lägger till bilder på en webbsida. En stor bild tar lång tid att ladda och det kan göra att webbsidan känns långsam. Det är därför viktigt att du anpassar bildstorleken så att den inte är större än vad den behöver vara.

Vill du minska bildstorleken kan du använda någon form av bildredigeringsprogram. Photoshop eller Paint funkar eller om du vill hitta något onlinealternativ så kan du prova det.

Kontrolla bildens upplösning och storlek genom att högerklicka på bilden och välja “Egenskaper”. Du kan även använda dig av en tjänst som heter [TinyPNG](https://tinypng.com/) för att minska bildstorleken.

### Versionshantering

Precis som tidigare så är det viktigt att du versionshanterar din kod. Det gör du genom att lägga till filerna i staging area, skriva en commit message och sedan pusha koden till GitHub. Se de tidigare instruktionerna för hur du gör det.

**Versionshanteringen är en historik för din kod. Det gör att du kan gå tillbaka till en tidigare version av din kod om du skulle behöva det.**

## CSS

Nu ska vi styla vår webbsida med hjälp av CSS. Vi kommer att använda oss av en extern CSS-fil för att styla webbsidan. Det gör vi för att det är ett bra sätt att separera HTML och CSS. Det gör det även enklare att arbeta med webbsidan.

Skapa en ny fil som heter style.css genom att klicka på “File” och sedan “New File”. Döp filen till style.css genom att klicka på “File” och sedan “Save As”. Skriv in namnet på filen och klicka på “Save”.

**Om du vill så kan du skapa en ny mapp som heter css och spara filen där. Precis som för bilderna så kan det hjälpa med strukturen för ditt projekt.**

Vi ska nu länka CSS-filen till HTML-filen. Det gör vi genom att lägga till en ```link``` tagg i ```head``` taggen. Det gör vi genom att skriva följande i ```head``` taggen.

```html
<link rel="stylesheet" href="style.css">
```

### Styla webbsidan

En bra start när du stylar en webbsida är att du lägger till lite marginaler, gör sidan mer lättläst och ändrar typsnittet.

Webbläsaren har en del inbyggda stilar och en del av dem kan vi behöver ändra på.

### Centera innehållet

För att centrera ditt innehåll på din webbsida ska vi göra ett par ändringar. Vi kommer att göra detta med hjälp av en CSS-regel. En CSS-regel består av en selektor och en deklaration. Selektorn bestämmer vilka element som regeln ska gälla för och deklarationen bestämmer hur elementen ska se ut.

När vi väl har skapat en CSS-regel så kan vi använda den flera gånger. För att göra det så behöver vi lägga till en klass på de element som ska använda CSS-regeln. Det gör vi genom att lägga till en ```class``` attribut på elementet.

**Ett element är en tagg i HTML.**

I ```style.css```
```css
.container {
  max-width: 60rem;
  margin-left: auto;
  margin-right: auto;
  padding-left: 2rem;
  padding-right: 2rem;
}
```

Öppna sedan ```index.html``` och redigera den.
Flytta rubriken och paragrafen in i en ```main``` tagg med klassen ```container```. Main taggen är en tagg som används för att markera huvudinnehållet på en webbsida.

I ```index.html```
```html
<main class="container">
  <h1>Min webbsida</h1>
  <p>Detta är min första webbsida</p>
</main>
```

Spara sidan och titta på den i webbläsaren, om du har Live Server igång så behöver du bara uppdatera sidan.

### Fixa bildstorleken

Bilden är för stor och tar för mycket plats på sidan. Vi ska nu ändra storleken på bilden med hjälp av CSS.

I ```style.css```
```css
img {
  max-width: 100%;
}
```

### Versionshantering

Precis som tidigare så är det viktigt att du versionshanterar din kod. Det gör du genom att lägga till filerna i staging area, skriva en commit message och sedan pusha koden till GitHub. Se de tidigare instruktionerna för hur du gör det.

### Typsnitt

Sidans typsnitt är standard-fonten som används av webbläsaren. Vi ska nu ändra typsnittet med hjälp av CSS. Det enklaste sättet att göra det är att ändra fonten i ```body``` taggen.

I ```style.css```
```css
body {
  font-family: sans-serif;
  font-size: 1.2rem;
}
```

Detta ändrar typsnittet till sans-serif och ändrar storleken på texten till 1.2rem. En rem är en enhet som används för att mäta storleken på text. En rem är lika stor som storleken på texten i ```html``` taggen.

### Annan font

Du kan självklart ändra till andra fonter, Visual Studio Code kan garanterat ge dig några förslag från ditt operativsystem. Men det är intressantare att prova någon font från en tjänst som [Google Fonts](https://fonts.google.com/).

På Google Fonts så kan du välja en font och sedan klicka på “Select this style” för att få en kodsnutt som du kan kopiera och klistra in i din CSS-fil. Du behöver även länka till fonten i ```head``` taggen i ditt HTML-dokument.

I ```style.css```
```css
body {
  font-family: 'Roboto', sans-serif;
  font-size: 1.2rem;
}
```

I ```index.html```
```html
<link rel="preconnect" href="https://fonts.gstatic.com">
<link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet">
```

Testa och prova en eller flera fonter. Hitta en som du tycker om och som passar till din webbsida.

Du kan även ange olika fonter för olika element med olika klasser. Det gör du genom att använda dig av en CSS-regel med en klass.

### Versionshantering

Du har nu gjort några ändringar, lägg till filerna i staging area, skriv en commit message som beskriver vad du har gjort/ändrat och pusha koden till GitHub.

### Test

* Vad är en CSS-regel och vad består den av?
* Vad behöver du göra för att använda din CSS i din HTML?
* Vad är en klass?

## Färger

Det är inte helt ovanligt att någon som du eller någon som jobbar på en hemsida vill ändra färger på element. För att göra det så använder du CSS och det styrs med egenskaperna ```color``` och ```background-color```.

### Ändra färg på rubriken

För att ändra färg på rubriken så behöver du lägga till en CSS-regel för ```h1``` taggen. Det gör du genom att skriva följande i ```style.css```.

```css
h1 {
  color: #333;
}
```

Du kan även skapa en klass för rubriken och använda den istället. Det gör du genom att lägga till en ```class``` attribut på ```h1``` taggen.

I ```style.css```
```css
.rubrik {
  color: #333;
}
```

I ```index.html```
```html
<h1 class="rubrik">Min webbsida</h1>
```

### Ändra färger på sidan

Testa att ändra färger på både text och bakgrund, lägg till mer innehåll och testa att ändra färg på det. Försök att vara noga med valet av färger så att din text är lättläst.

Vill du prova att skapa färgscheman kan du testa ett verktyg som heter [Coolors](https://coolors.co/).

### Versionshantering

Nu är det dags igen, du kommer förhoppningsvis ihåg hur du versionshanterar din kod. Lägg till filerna i staging area, skriv en commit message som beskriver vad du har gjort/ändrat och pusha koden till GitHub.

## Hypertext och länkar

HTML står för Hypertext Markup Language. Hypertext är text som innehåller länkar till andra dokument. Det är det som gör webben till webben. Vi ska nu lägga till en länk till en annan sida.

### Länka till en annan sida

Vi ska nu lägga till en länk till en annan sida. Det gör vi genom att använda en ```a``` tagg. ```a``` taggen är ett anchor-element som används för att skapa länkar. I taggen så behöver vi ange en ```href``` attribut som innehåller länken (url) till sidan som vi vill länka till.

```html
<a href="https://www.google.com">Google</a>
```

Lägg till länken i ```index.html``` och spara filen. Titta på sidan i webbläsaren och testa länken.

### Länka till en annan sida i samma mapp

Vi ska nu lägga till en länk till en annan sida i samma mapp. Du behöver först skapa en ny fil som heter about.html genom att klicka på “File” och sedan “New File”. Döp filen till about.html genom att klicka på “File” och sedan “Save As”. Skriv in namnet på filen och klicka på “Save”.

```html
<a href="about.html">Om</a>
```

Lägg till länken i ```index.html``` och spara filen. Titta på sidan i webbläsaren och testa länken.

Redigera sedan ```about.html``` och lägg till en länk tillbaka till ```index.html```.

```html
<a href="index.html">Tillbaka</a>
```

### Viktigt

Glömt inte att lägga till den grundläggande HTML-strukturen för en webbsida i ```about.html```. Du gör det genom att skriva ```html:5``` och sedan trycka på tabb-tangenten precis som för index sidan. 

När det är gjort kan du redigera innehållet och länka till CSS-filen precis som för index sidan.

### Versionshantering

Du börjar kunna det här och vanan att versionshantera din kod börjar sätta sig. Lägg till filerna i staging area, skriv en commit message som beskriver vad du har gjort/ändrat och pusha koden till GitHub.

## Test

* Hur använder du en ```a``` tagg för att skapa en länk?
* Vad heter egenskapen för anchor-elementet som används för att skapa länkar?
* Vad är en url?

## Skapa innehåll

Nu är det upp till dig att skapa innehåll till din webbsida. Du kan skapa en sida om dig själv, en sida om något du tycker om eller något annat som du tycker är intressant.

På om sidan så lägger du till en länk till ditt GitHub repository och en länk till din GitHub profil.

## Hosting med GitHub Pages

Nu ska vi hosta din webbsida med hjälp av GitHub Pages. GitHub låter oss använda repositoryt som en webbserver. Det gör att vi kan visa upp vår webbsida på internet.

Surfa till ditt repository på GitHub och klicka på “Settings”. Scrolla sedan ner till “GitHub Pages” och klicka på “Source”. Välj “main” och klicka på “Save”.

Det kan ta några minuter innan din webbsida är tillgänglig. När den är det så kan du surfa till ```https://<användarnamn>.github.io/<repository>```.

## Versionshantering

Om du önskar att styra över vilken version av din hemsida som visas upp på GitHub Pages så kan du använda dig av en branch. En branch är en kopia av ditt repository som du kan göra ändringar i utan att påverka originalet. Du kan sedan skapa en pull request för att föreslå ändringar till originalet.

För att skapa en branch så klickar du på “Branch: main” och skriver in ett namn på din branch. Klicka sedan på “Create branch”.

Du kan nu göra ändringar i din branch och sedan skapa en pull request för att föreslå ändringar till originalet.

## Skapa fritt

Nu har du verktygen för att skapa en webbsida. Det finns brappiljarder av instruktioner och tutorials på nätet som du kan använda dig av för att lära dig mer.