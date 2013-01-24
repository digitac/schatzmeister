Vorwort
=============

Schatzmeister ist die freie Mitgliederverwaltung und Buchhaltungssoftware des Aachener Vereines "Digitales Aachen"

Ich habe sehr lange darüber nachgedacht ob das Projekt in Englisch oder in Deutsch sein soll.
Normalerweise wähle ich als Projektsprache Englisch. Zum einen, weil diese Sprache -gerade für die Programmierung-
sehr elegant ist zum anderen weil praktisch jeder den Code lesen kann.

Da es sich hier aber um Buchhaltungssoftware handelt, die vor allem den Deutschen Gesetzen genügen soll und 
die Buchhaltungs-Vokabeln oft nicht so einfach ins Englische übersetzbar sind habe das kompette Projekt in
Deutscher Sprache gehalten.

Die Software wurde bereits im Jahr 2012 begonnen. Und aus Gewohnheit natürlich in Englischer Sprache.
Deshalb ist der // erste // checkin ohne History bereits weit fortgeschritten.

Da ich nachträglich alles ins "Deutsche" übersetzt habe wird das Projekt zu Beginn etwas verwirrend. 
Module die allgemeinen Charakter haben führe ich weiter auf Englisch fort (wie zum Beispiel das SMTP-Modul).

In diesem Sinne bitte ich auch teilnehmende Entwickler fortzufahren. 

Um GIT-Konflikte beim syncen zu vermeiden und das Projekt so weit wie möglich verwaltbar zu halten gelten erwarte ich,
dass folgende Regeln eingehalten werden. Pull Requests, die Konflikte aufzeigen, die durch Nicht-Einhaltung dieser Regeln 
entstehen muss ich aus Zeitgründen ablehnen.

Es wird darum gebeten alle Module die speziell mit der Deutschan Rechtsprechung und Buchhaltung zusammenhängen auch in 
deutscher Sprache zu entwickeln. Alle Helper, Tools und alles was der Community im Allgemeinen dienen kann bitte
ich in englischer Sprache zu formulieren, zu programmieren und zu kommentieren.

Ich gehe davon aus, dass jeder deutsch sporechende Programmierer auch fließend englisch spricht. Daher wird der 
englsische Teil nicht ins Deutsche übersetzt.

Ich hoffe auf eine produktive Zusammenarbeit und auf eine Software, die endgültig und nachhaltig das "Softwareproblem"
für Mitgliederverwaltungen endgültig löst.


Diese Software wird von unserem Verein von Zeit- zu Zeit zu einem Symbolischen Verkaufspreis im Apple App-Store
angeboten. Wir sind ein Allgemeinnütziger Verein und möchten gerne alle an dieser Software teilhaben lassen.
Da Apple die iCloud-Funktionialität nur über den Appstore anbietet, werden wir die Software auch unter unserem
Apple-Account veröffentlichen. Da der Developer-Account jählich Geld kostet, werden wir die Software für den
im App-store minimalen Preis anbieten. Auf diese Weise können wir die Kosten tragen.
Jeder Überschuss wird als allgemeine Spende für unseren Verein verstanden. Wir verwenden die Spenden
um weitere Projekte fortzuführen und die "Digitale Kultur" voranzutreiben.

Wir verweisen wir auf den Lizenz-Text im Anhang. Der Verein Digitac behält es sich alleine
vor diese Software in den AppStore einzustellen. Sollte die Finanzierung gesichert sein geben wir diese Software auch frei.
Ansonsten erlauben wir Jedermann an dieser Software teilzunehmen, den Sourcecode frei zu verwenden. Unter gewissen 
Einschränkungen ist auch eine kommerzioelle Nutzung gestattet (Lediglich der Name "Schatzmeister" und das "Logo" der 
Software unterliegt unserem Copyright und Urheberrecht.

Als Gegenleistung für den App-Preis erhält jeder Updates, verfügt über iCloud-Backups und Datasync.
Diese App wird es für OS X, iPhone und iPad geben.

Eine Portierung auf die Platformen "Android", "Windows Phone" und Windows gestatten wir ausdrücklich.
Allerdings stellen wir die Bedingung, dass die portierten Version ebenfalls open source sind und dass
die Softwareprojekte immer im Kontext mit diesem Reository geführt werden.



schatzmeister
=============

Schatzmeister wird als "Agile Vereinsbuchhaltungssoftware" gestaltet.
Die Idee für diese Software wurde aus der Not geboren, dass auf dem Markt aus unserer Sicht keine wirklich
gute Vereinssoftware verfügbar ist und man immernocjh "Buchhalter" sein muss um die Vereinskasse zu führen.

Die Vision ist es ein Programm zu entwickeln, dass verteilt typische Vereinsabrechnungen automatisiert und
Vorgangsweise umsetzt. So soll der Schatzmeister/Kassenwart den Schrecken vor der Buchhaltung verlieren und 
auch ohne Know- How legal handeln können.

Beitragsbuchungen werden bei den Mitgliedern geführt. Sachgegenstände werden im Inventar eingetragen. 
Barzahlungen in der Kasse.

Der Schatzmeister wählt aus einer Lichte von "Vorgaben" was er da macht. So werden Gegenstände
automatisch als Vermögen gebucht, gerinfügige Wirtschaftsgüter werden sofort abgeschrieben und so weiter.

Im späteren Verlauf soll ein Editor Buchhaltern und Steuerexperten die Möglichkeit geben die Kontenpläne
Buchungsvorlagen und steuerrechtliche Regeln einzugeben, so dass der Schatzmeister // immer // die richtige
Buchhaltung macht. Hier liegt das Augenmerk aber nicht auf einer "optimalen Bilanzgestaltung" sondern
auf eine Fehlerfreie verbuchung gegenüber dem Finazamt. Die Software soll dem Schatzmeister die Möglichkeit geben
sich nur noch um siene Mitglieder zu kümmern, statt stundenlang die Buchhaltung zu machen.

Schatzmeister ist die Agile Kompettlösung für Vereine die dann auch Nicht-Buchhalter zum Schatzmeister wählen können.

Das schäne an dieser Software ist aber: Es kommt am Ende tatsächlich eine Dreigliedrige Buchhaltung mit Kontenrahmen
SKR 49 raus. Spendenbescheinigungen werden nach aktuellem Recht ausgegeben.

Für die Korrektheit der Daten haften die Entwickler nicht. Wir bieten später eine Schnittstelle, die von Steuerrechtlern
gefüllt werden kann.

Diese Software hat ein Userinterface das auf das iPad optimiert ist und einem 4-Click-Paradigma entspricht. 
Wir möchten, dass // jeder // Vorgangnach maximal drei Bildschirmberührungen erreichbar ist. Wir wollen,
dass die lästigen steuerrechtlichen Vorgänge so weit wie möglich automatisiert sind,
damit sich der Vorstand ganz auf seine Aufgaben kümmern kann: Der Verein und seine Mitglieder.


Designrichtlinien
=============

Um fireden mit GIT zu haben werden folgende Code-Vorschriften angenommen:

1. Code-Signaturen bitte ohne Space:
Beispiel:
-(NSArray*) sortedFiles {

Falsch:
- (NSArray*) sortedFiles {


2. Bitte Klammern IMMER hinter die Signatur mit einem Space, gefolgt von einer Leerzeile
Beispiel:
-(NSArray*) sortedFiles {

  //Code
}

Falsch:
-(NSArray*) sortedFiles
{
}

oder

-(NSArray*) sorted Files {
  // Code
}

Dasselbe gilt für ALLE Anweisungen wie if, elseif, while, etc.

if (condition) {

  // code
}

3. if-Anweisungen IMMER voll klammern

if (condition) {

  // branch1
} else {

  // branch2
}

Falsch:
if (condition) branch1
else branch2;

4. Proerties bitte nuir in einem EIntrag pro Zeile
@property (nonatomic, strong) NSString* eintrag1;
@property (nonatomic, strong) NSString* eintrag2;

Falsch:
@property (nonatomic, strong) NSString* eintrag1, eintrag2;


Durch Anwendung dieser Regeln verhindern wir Konflikte. Ich bitte um Einhaltung.


Wir implementieren ausschließlich mit ARC (Automatic Reference Count) Bitte also nur "strong", nie "retain" verwenden.
Bitte keine Threads benutzen, sondern dispatch_queues.


Kommentare bitte im Appledoc-Style.

BeBopp

