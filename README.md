# technisch-ontwerp
## Projectvoorstel (updated) groep IK07
##### Samenvatting
Op deze (sport) trivia website kunnen gebruikers spelen tegen vrienden, kennissen of willekeurige tegenstanders. Deze (sport) trivia site stimuleert zijn gebruikers om zelf mee te denken in het maken van vragen en deze dan ook daadwerkelijk te maken. Er zijn leaderboards die continu bijhouden welke gebruikers het beste presteren op het gebied van vragen beantwoorden, maar ook op het gebied van vragen maken en beoordelen. 

##### Features
* Gebruikers moeten zich kunnen aanmelden met Facebook of e-mail en vervolgens een username en wachtwoord kunnen kiezen.
* Na registratie kunnen gebruikers inloggen met de door hun gekozen methode bij de registratie.
* Gebruikers kunnen een trivia Quiz starten. 
* Gebruikers kunnen kiezen of ze 1 tegen 1 of 2 tegen 2 willen spelen. 
* Gebruikers kunnen tegen Facebook vrienden spelen, of een username zoeken om hier tegen te spelen. 
* Gebruikers kunnen ook tegen een willekeurige tegenstander spelen. 
* Gebruikers kunnen hun eigen trivia vraag toevoegen aan de database. Dit gebeurt volgens dit proces:
** De gebruiker typt de gewenste vraag en kiest een bijbehorende categorie
* De vraag komt op een pagina terecht waar andere gebruikers de vraag kunnen beoordelen van 1 tot 5 sterren. Andere gebruikers kunnen ook suggesties doen om de vraag te verbeteren.
* Een moderator houdt deze pagina in de gaten en voegt eventueel goed beoordeelde vragen toe aan de database.
* Eenmaal toegevoegd aan de database, komt de vraag terecht in trivia games van gebruikers.
* Ongepaste vragen moeten gereport kunnen worden door gebruikers, de moderator bepaald vervolgens of ze verwijdert worden en of de maker van de vraag geband wordt. 
* Er zijn leaderboards die bijhouden hoeveel vragen de gebruikers hebben toegevoegd, hoe vaak de gebruikers andere vragen hebben ‘gerate’ (beoordeeld), hoeveel van hun vragen zijn ‘gerate’ door anderen, hoeveel suggesties zij hebben gedaan om andermans vragen te verbeteren. 
* De gebruiker heeft een profiel met statistieken, hierin wordt geregistreerd hoe vaak hij/zij gewonnen heeft en hoeveel procent van de vragen hij/zij goed heeft. 
* Er zijn leaderboards waarin wordt bijgehouden welke gebruikers de meeste ‘wins’ hebben en welke gebruikers het hoogste percentage goede antwoorden geven. 
* Gebruikers moeten kunnen uitloggen. 
* Gebruikers moeten zich kunnen aanmelden met Facebook

##### Minimum viable product. 
* Gebruikers moeten zich kunnen aanmelden met e-mail en vervolgens een username en wachtwoord kunnen kiezen.
* Na registratie kunnen gebruikers inloggen bij de inlog pagina.
* Gebruikers kunnen een trivia Quiz starten en krijgen feedback of het antwoord goed of fout was. 
* De vragen komen uit een online database, deze is geïntegreerd in onze website. 
* Gebruikers kunnen tegen iemand spelen, niet real-time. 
* Gebruikers kunnen tegen andere usernames spelen. 
* Gebruikers kunnen ook tegen een willekeurige tegenstander spelen. 
* Gebruikers kunnen hun eigen trivia vraag insturen, deze wordt beoordeeld door de moderator en toegevoegd wanneer deze ‘goed genoeg is’.
* Gebruikers moeten hun account kunnen aanpassen, bijv. hun email. 
* Gebruikers moeten kunnen uitloggen.

##### De website slogan.
Trivia; Create, Play, Compete. 
Deze is kort opgezet zodat de website een mooie simpele opening heeft op de homepagina. Hierdoor zullen mensen de website mogelijk beter onthouden. 

##### Extra features voor eventuele uitbreiding.
Vragen op basis van opkomende sports events, hiermee wordt bijvoorbeeld bedoeld, de Olympische Winterspelen? → Allemaal vragen hierover.
Uiteindelijk moet het een geautomatiseerd process worden waar de community de website gaat vernieuwen en verbeteren door vragen toe te voegen. Hierdoor hoeft er niet meer naar de website gekeken te worden door moderators. De vragen worden bij een bepaalde rating (waar deze vraag boven of op is blijven hangen voor een gedefinieerde periode) in een database gegooid. 
##### Afhankelijkheden
Voor het bouwen van onze gewenste webapplicatie zijn wij afhankelijk van een aantal onderdelen:
De basis van onze verzameling trivia-vragen zal afkomstig zijn uit online databases. Wij zullen deze natuurlijk filteren zodat wij alleen vragen toevoegen aan onze eigen database die bij onze niche horen: sport. Om een zo’n groot mogelijk scala aan vragen te verzamelen zullen we wellicht meerdere online databases moeten raadplegen. Twee voorbeelden van databases die we kunnen gebruiken zijn opentdb.com en jservice.io.
(optioneel) Om gebruikers te kunnen laten inloggen door middel van Facebook, hebben wij de Facebook API nodig: https://developers.facebook.com/docs/facebook-login/web
Voor het design van de website zullen wij hoogstwaarschijnlijk ook gebruik gaan maken van icoontjes. Deze kunnen we natuurlijk zelf creëren met bijvoorbeeld Adobe Illustrator, maar het gemakkelijkst is om hiervoor een online database te gebruiken zoals https://www.flaticon.com/.

##### Het raamwerk van de website zal bestaan uit twee componenten:
Bootstrap (https://getbootstrap.com/) voor de front-end, wat het vormgeven van de website zoals de gebruiker die ziet flink zal versimpelen.
Flask (http://flask.pocoo.org/) voor de back-end, wat het koppelen van de Python code met de front-end van de website mogelijk zal maken.
Er zijn vele andere trivia games te vinden op het web. De drie websites die bovenaan Google staan als we zoeken op ‘trivia game’ zijn triviaplaza.com, sporcle.com en funtrivia.com. Deze kunnen dus wel worden gezien als de grootste - of op zijn minst de makkelijkst vindbare - trivia websites. Wij gaan ons van deze websites onderscheiden op de volgende vlakken:
 Design: elk van deze websites heeft een verouderd design. Onze website zal er strakker uitzien en daarom de gebruikers van tegenwoordig eerder aanspreken.
Competitiviteit: bij elk van deze websites speelt de gebruiker tegen zichzelf. Wij willen de competitiviteit stimuleren door gebruikers de mogelijkheid te geven om tegen vrienden te spelen.
Niche: alhoewel het bij elk van deze websites mogelijk is quizzes uit te kiezen per niche, hebben wij ervoor gekozen om onze hele website rond het thema ‘sport’ te bouwen. Hierdoor kunnen wij onze focus geheel leggen op één duidelijke doelgroep, namelijk geïnteresseerden in sport.
Naar ons idee zal het ontwikkelen van de volgende onderdelen van onze webapplicatie de grootste uitdaging zijn:
Databases: aangezien wij nog geen ervaring hebben met programmeren rondom databases, zal het een uitdaging worden om onze trivia-database te vullen met niet alleen vragen uit API’s, maar ook met user-generated vragen.
Flask: ook hebben wij nog weinig tot geen ervaring met het koppelen van een back-end met een front-end door middel van een framework. Dit wordt veel uitzoekwerk.
Competitiviteit: het zal een uitdaging worden om de interactie tussen twee spelers die met elkaar een spel spelen te realiseren. Als de ene speler namelijk zijn of haar beurt gespeeld heeft, is diegene afhankelijk van het resultaat van de andere speler om te weten of het spel gewonnen is of niet. De informatieoverdracht tussen de twee spelers en de feedback die wij daarbij geven moet vlekkeloos verlopen.

##### Sanity check. 
Leerdoelen van het programmeer project in teams van drie studenten (60%)

Eisen
leren hoe je de functionaliteit van een nieuwe website kunt vastleggen ✔
leren hoe je een technisch ontwerp maakt voor een grotere website ✔
leren hoe je met meerdere mensen code voor een website kunt delen via Git ✔
kennis maken met het werken in teamverband en projectmatig werken ✔
leren hoe je een project kunt opdelen om een tijdsplanning te maken ✔
Trivia. Gebruikers kunnen triviavragen beantwoorden en op die manier punten scoren. Er is een interessant systeem om van andere gebruikers te winnen. De vragen komen uit een online triviadatabase zoals http://jservice.io. ✔

Beoordelingscriteria
Omvang — is het een samenhangend en compleet product? ✔
Bruikbaarheid — is het product goed te gebruiken voor beginners en gevorderden? ✔
Ontwerp — hoe overzichtelijk en gestructureerd zijn de code en database? ✔
Stijl — hoe leesbaar is de code? ✔

Voor al deze punten is gechecked of het project er aan zal kunnen voldoen. Er is geconstateerd dat dit zo is. De sanity check is doorstaan en het project concept kan gemaakt worden. Mogelijk worden features en andere aspecten uit dit voorstel tijdens het proces aangepast.

##### Views
De views file is een te groot bestand om hierin te verwerken, daarom wordt er een link verschaft naar het desbetreffende document. 
"https://drive.google.com/open?id=1eBlgCs6AY-EOdhr9N6GonxqVlYeD5ZtY"

##### Controllers
Home
index.html is de pagina die de gebruiker als eerste ziet als de website wordt bezocht. Op deze homepage staan onze slogan, een korte uitleg van het spel en natuurlijk knoppen naar de “Sign up” en “Log in” pagina’s.
```sh
@app.route("/")
def index():
    return render_template("index.html")
```

Sign up
Op deze pagina kan de gebruiker zich aanmelden door middel van e-mail, gebruikersnaam en wachtwoord. Als alle gegevens correct zijn ingevuld, komt de gebruiker op de “Log in” pagina terecht, waar de gebruiker met de zojuist aangemaakte gegevens op onze website kan inloggen. Als de gegevens niet correct zijn ingevuld, laadt de “Sign up” pagina opnieuw (zo mogelijk met een error message) en krijgt de gebruiker nog een keer de kans om zijn gegevens correct in te voeren.
```sh
@app.route("/signup", methods = ["GET", "POST"])
def signup():
    # user is on signup page and fills in form
    if request.method == "POST":
        # check conditions for unsuccessful signup
        """
        if ... :
            return redirect(url_for("signup"))
        """
        
    # signup was successful
    return redirect(url_for("login"))

    # user reaches signup page via link or redirect
    if request.method == "GET":
        return render_template("signup.html")
```

Log in
Op deze pagina kan de gebruiker inloggen, indien deze zich al een keer heeft aangemeld. Als de ingevoerde gebruikersnaam en het wachtwoord kloppen met de gegevens uit de database, komt de gebruiker op de “Play” pagina. Hier is het mogelijk om een spel te starten. Als de ingevoerde gegevens niet kloppen met de database, laadt de “Log in” pagina opnieuw (zo mogelijk met een error message) en krijgt de gebruiker nog een keer de kans om zijn gegevens correct in te voeren.
```sh
@app.route("/login", methods = ["GET", "POST"])
def login():
    # user is on login page and fills in form
    if request.method == "POST":
        # check conditions for unsuccessful login
        """
        if ... :
            return redirect(url_for("login"))
        """
            
        # login was successful
        return redirect(url_for("play"))
            
    # user reaches login page via link or redirect
    if request.method == "GET":
        return render_template("login.html")
```
NOTE: Na ingelogd te zijn krijgt de gebruiker standaard een website header met navigatie te zien. Hier kan je navigeren tussen de “Play”, “Create”, “Leaderboard” en “Profile” pagina’s. Uiteraard is het via deze navigatie ook mogelijk om uit te loggen.

Play
Nadat de gebruiker is ingelogd, komt hij/zij op een pagina met een grote PLAY knop. Als op deze button geklikt wordt, gaat de gebruiker naar question.html. Hier start het spel en krijgt de gebruiker een triviavraag te zien die binnen 10 seconden beantwoord moet worden.
```sh
@app.route("/play", methods = ["GET"])
def play():
    return render_template("play.html")
```

Question
Hier wordt de “Question” pagina geladen. Deze toont een willekeurige vraag uit de database met de vier bijpassende multiple choice antwoorden. 
```sh
@app.route("/question", methods = ["GET", "POST"])
def question():
    # user is on question page and selects an answer
    if request.method == "POST":
        # check if question was answered correctly
        """
        if ... :
            return.render_template("correct.html")
        else:
            return.render_template("false.html")
        """
	
    if request.method == "GET":
        return render_template("question.html")
```

Create 
```
@app.route(“/create”, methods = [“GET”, “POST”]
def create():
    # user clicks one of the buttons
    if request.method == “POST”:
        # use HTML buttons with the ‘name’ and ‘value’ attributes
        if request.form[“choice”] == “create”:
            return render_template(“create_question.html”)
        elif request.form[“choice”] == “rate”:
            return render_template(“rate_question.html”)
    if request.method == “GET”:
        return render_template(“create.html”)
```

Create_question
```
@app.route(“/create_question”, methods = [“GET”, “POST”]
def create_question():
    # user clicks on submit button
    if request.method == “POST”:
        “””
        Store user entry in database
        “””
        return redirect(url_for(“create_question”))
     
    if request.method == “GET”:
        return render_template(“create.html”)
```

Leaderboard
```
@app.route(“leaderboards”, methods = [“GET”]
def leaderboards():
    render_template(“leaderboards.html”)
```

Profile
```
@app.route(“profile”, methods = [“GET”, “POST”]
def profile():
    if request.method == “POST”
        # user wants to change profile information
        return render_template(“settings.html”)	
    if request.method == “GET”:
        return render_template(“profile.html”)
```

##### Models/helpers
Deze functies hieronder komen in onze helpers.py
```
def apology(message, code=400):
```
Er is een apology message nodig die een error aangeeft wanneer deze ontstaat. Handig om te zien wanneer een error voor komt en om de usability te verbeteren. 
```
def login_required(f):
```
Login is nodig voor alle acties na het login scherm, dus bijvoorbeeld voor play of create. Hier moet een user bekend zijn zodat zijn vragen ook beoordeeld kunnen worden. En alle acties kunnen tevens pas uitgevoerd kunnen worden nadat de user is ingelogd. 
```
def generate_question():
```
Een vraag moet uit de api gehaald kunnen worden of uit het create database. Zodat de vragen random worden gekozen uit de API of het database. 
```
def get_random_answer
```
Deze functie moet voor drie verschillende buttons constant worden aangeroepen. Deze worden opgevraagd wanneer de trivia bezig is. 

Deze functies zullen in de application.py zitten
```
def register():
```
Een user moet kunnen registeren voor de website, dit moet worden opgeslagen in het database
```
def logout():
```
De user moet kunnen uitloggen en de sessie moet worden gecleared. 
```
def login():
```
De user moet kunnen inloggen, de sessie moet worden gesaved. 
```
def get_statistics():
```
De statistieken van alle spelers worden opgehaald en in een rekensom gegooid, deze bepaald hun ranking in de leaderboards. 

##### Plugins en frameworks
Er wordt gebruikt gemaakt van de jService API, dit is een database met meer dan 156.800 trivia vragen. We proberen deze vragen te filteren op sportvragen, aangezien we een sport trivia website willen bouwen. Echter nemen we in onze MVP (minimum viable product) genoegen met het implementeren van de gehele database in onze website. (http://jservice.io)
Verder wordt voor het bouwen van deze trivia website gebruik gemaakt van het Bootstrap framework. Bootstrap is een framework die bestaat uit een verzameling hulpmiddelen voor het maken van een website. In dit project wordt Bootstrap gebruikt om verschillende templates te bouwen, om zo tijd te besparen. Deze tijd zal vervolgens geïnvesteerd worden in het werken aan andere details van de website, namelijk het afmaken van de MVP. (https://getbootstrap.com/docs/4.0/getting-started/introduction/)
Ook wordt het Flask framework gebruikt, dit is een python ‘microframework’. Flask is een tool die, net als Bootstrap, helpt bij het maken van templates voor een website. Flask en Bootstrap zorgen er beiden voor dat een website consistent blijft in de stijl waarin deze gemaakt is. Dit werkt tijdsbesparend en verhoogt de kwaliteit van ons project, aangezien we over een korte tijdsperiode beschikken. (http://flask.pocoo.org)


