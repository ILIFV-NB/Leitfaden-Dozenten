<!--
author:   Nancy Brinkmann, Ronny Stolze

email:    nancy.brinkmann@h2.de, ronny.stolze@h2.de

version:  1.0.0

language: de

narrator: DE FEMALE

comment:  Try to write a short comment about
          your course, multiline is also okay.

script:  https://cdnjs.cloudflare.com/ajax/libs/echarts/4.2.1/echarts-en.js

-->

# Allgemeines

Im Folgenden finden Sie zwei Leitfäden für je einen Schnelleinstieg in [LIA-Script](#2) sowie die [Webumgebung eLab](#20).

[LIA-Script](https://liascript.github.io/) ist eine von André Dietrich entwickelte erweiterte Markdownsprache, mithilfe derer Sie Ihren Kurs ohne Programmierkenntnisse aufbauen können. Auf den folgenden Seiten bekommen Sie einen Überblick über das Arbeiten mit LIA-Script. Darüber hinaus erfahren Sie in der [Dokumentation](https://liascript.github.io/course/?https://raw.githubusercontent.com/liaScript/docs/master/README.md#1) (englisch) alles, was Sie über LIA-Script wissen müssen und, was Sie damit anstellen können. Eine verkürzte Version auf Deutsch finden Sie [hier](https://liascript.github.io/course/?https://raw.githubusercontent.com/liaScript/demo/master/README.md#1).

Die [Webumgebung eLab](https://elab-hsmd-qa.dev.enterprises/) ist eine Plattform, auf der Sie Ihre Kurse einbinden, online verfügbar machen und ggf. Bearbeitungsstände einsehen können.

Hier finden Sie eine Orientierungshilfe für eLab:

[preview-lia](https://raw.githubusercontent.com/ILIFV-NB/Orientierungshilfe-eLab/master/README.md)


# ~~**Schnelleinstieg LIA-Script**~~

Die folgende Beschreibung stellt lediglich einen ~~kurzen~~ Einblick in die Erstellung eines Kurses mit LIA-Script dar. An dieser Stelle sei noch einmal auf die komplette (englische) Beschreibung und Auflistung der Möglichkeiten mit [LIA-Script](https://liascript.github.io/course/?https://raw.githubusercontent.com/liaScript/docs/master/README.md#1) verwiesen.

Bevor Sie einen Kurs erstellen können, sind einige [Vorbereitungen](#3) zu treffen. Eine Anleitung finden Sie auf den nächsten Seiten.


## **Vorbereitungen**

Als Grundlage für den Inhalt Ihrer Kurse benötigen Sie eine Textdatei, in der Sie Ihren gesamten Kurs aufbauen. Zum Bearbeiten dieser eignet sich z.B. der Editor [Atom](https://atom.io/). Denn hier haben Sie mithilfe von aktuell zwei Werkzeugen für LIA-Script (Plugins: [liascript-preview](https://atom.io/packages/liascript-preview) und [liascript-snippets](https://atom.io/packages/liascript-snippets)) die Möglichkeit, eine Preview Ihres Kurses anzusehen bzw. mit kurzen Eingaben Befehle zu finden, die Sie bspw. beim [Einbinden von Medien](#7) unterstützen. (Näheres zu den Plugins finden Sie [hier](#26).)

Um Ihre Kurse online zur Verfügung stellen zu können, nutzen wir eine Plattform: [GitHub](https://github.com/). Mithilfe dieser Plattform sind Sie in der Lage, Ihre Kurse samt Medien zu verwalten, Sie gemeinsam mit Kollegen zu bearbeiten sowie Abzweigungen zu erstellen, wenn Sie sich einmal nicht sicher sind, in welche Richtung Ihr Format gehen soll.

Die folgenden zwei Seiten unterstützen Sie bei den Vorbereitungen.

<br/>
* Versionsverwaltung [GitHub](#4)
* Online Editor [Atom](#5)


### GitHub

<br/>
1. Account auf [GitHub](https://github.com/) anlegen

Um Kurse online zur Verfügung zu stellen, benötigen Sie eine Plattform (bspw. GitHub), auf der Sie Ihre Kurse in sogenannten Repositories verwalten. Der erste Schritt ist also, auf der Website von GitHub einen **Account** anzulegen.

<br/>
2. **Repository** erstellen $ ^* $ (inkl. ReadMe-Datei)

Wenn Sie auf GitHub angemeldet sind, finden Sie auf der Seite rechts oben ein $+$-Zeichen. Im Dropdown-Menü klicken Sie auf *New repository*. (Alternative: Nach Klick auf das GitHub Logo/Katzensymbol in der linken oberen Ecke, erscheint ein *New*-Button.) Hier vergeben Sie einen (Kurs-)Namen, geben optional eine kurze Beschreibung ein und entscheiden, ob das **Repository** gleich öffentlich sein soll oder zunächst privat$ ^{* * } $. Um direkt eine ReadMe-Datei (Textdatei) zu erstellen, die Sie als Grundlage für Ihren Kursinhalt benötigen, setzen Sie vor *Initialize this repository with a README* einen Haken. Mit *Create repository* bestätigen Sie Ihren Vorgang. Ihr Repository wird nun auf der Seite links oben nach Klick auf das GitHub Logo sichtbar.

<br/>
3. Fotos und Videos hochladen (oder später lokal)

Nachdem Sie Ihr Repository geöffnet haben, sehen Sie einen Button mit dem Namen *Upload files*. Hierüber können Sie per 'Drag & Drop' **Fotos oder Videos laden**, die Sie in Ihren Kurs einbinden möchten. Es empfiehlt sich, diese in Ordnern abzulegen, die bspw. die Namen *images* bzw. *movies* tragen. Sie können diesen Schritt aber auch später lokal über Ihren Rechner ausführen. (Erläuterungen unter GitHub -> 4. bzw. Atom -> 3.)

<br/>
4. Repository für Atom **klonen**

Sie haben nun die Möglichkeit, Ihren Kurs im Online-Editor Atom zu laden und dort zu bearbeiten. Öffnen Sie dazu ihren Kurs auf GitHub, klicken rechts über Ihrem Kurs auf *Code* und kopieren Sie den Link. Mithilfe dieses Links werden die Inhalte des Repositorys lokal auf Ihrem Rechner gespeichert und können dort mit Material befüllt werden (Alternative -> direkt in GitHub). Für nähere Erläuterungen und die weitere Vorgehensweise schauen Sie sich bitte das Kapitel [Atom](#5) -> *3. Geklontes Repository laden* an.

<br/>
$^* $ [Hier](https://guides.github.com/activities/hello-world/) finden Fortgeschrittene nähere Informationen zum Erstellen und Bearbeiten eines Repositorys.

$^{* * } $ Ihr Kurs wird erst dann für andere zugänglich sein, wenn Sie den Status auf 'public' umgestellt haben.

### Atom

<br/>
1. Online Editor [Atom](https://atom.io/) **installieren**

Laden Sie sich den Online-Editor Atom herunter und installieren Ihn auf Ihrem Rechner. In Atom können Sie Ihre Textdateien (ReadMe) mit den Inhalten Ihres Kurses bearbeiten und mithilfe von zwei LIA-Script Plugins (siehe Punkt 2) eine Preview Ihres Kurses einblenden sowie mit Eingabe des Wortes *lia* eine Reihe von Befehlen finden, die Sie bspw. beim [Einbinden von Medien](#7) unterstützen.

<br/>
2. [Plugins](https://atom.io/packages/search?utf8=%E2%9C%93&q=liascript&commit=Search) (Werkzeuge) für LIA installieren

Nach Eingabe der Tastenkombination **Strg$+$Shift$+$P** geben Sie in die Suchleiste  ~~settings~~ ein und scrollen solange herunter bis *Settings View: Install Packages and Themes* erscheint. Hier geben Sie in die Suchleiste ~~liascript~~ ein. Es erscheinen aktuell die zwei Plugins *liascript-preview* und *liascript-snippets*, die Sie installieren sollten. Näheres zu den Plugins und deren Installation finden Sie [hier](#26).

<br/>
3. Geklontes **Repository laden**

Nachdem Sie Ihr Repository (wie unter GitHub -> 4. *Repository für Atom klonen* beschrieben) geklont haben, wechseln Sie zu Atom, geben nach Eingabe der Tastenkombination **Strg$+$Shift$+$P** ~~clone~~ in die Suche ein und bestätigen mit *Enter*. Unter *clone from* fügen Sie Ihren Link ein und passen unter *to directory* ggf. ihren Pfad an. Dort werden Sie ab sofort alle Ordner und Dateien bzgl. Ihres Kurses finden und können Bilder und Videos hinzufügen oder entfernen.


## **Textdatei erstellen**

Ihre geklonten Repositories finden Sie nun links im 'Projektbaum' in Atom. Dort öffnen Sie die zu bearbeitende ReadMe-Datei$^* $ mit einem Klick darauf und anschließend die Preview mit der Tastenkombination **Alt$+$L**. Diese Textdatei versehen Sie z.B. mit folgendem Kopf$^{**} $:

```XML
<!--
author:   Your Name

email:    your@mail.org

version:  0.0.1

language: de_DE

narrator: DE FEMALE

comment:  Try to write a short comment about
          your course, multiline is also okay.

-->
```

Tragen Sie hier Ihren Namen und Ihre E-Mail Adresse sowie einen kleinen Kommentar zu Ihrem Kurs ein.

Daran anschließend generieren Sie Ihr Inhaltsverzeichnis$^{**} $, indem Sie vor jede Überschrift eine # setzen, und vor jede weitere Überschrift, die der oberen zuzuordnen ist, zwei ## usw. Zwischen Ihren Überschriften platzieren Sie ihre Texte, [Bilder](#8), [Videos](#9) oder [Links](#10). Um Absätze kenntlich zu machen, fügen Sie eine Leerzeile zwischen zwei Textblöcken ein. Für Aufzählungen stellen Sie dem jeweiligen Anstrich einen Stern $ * $ mit einem Leerzeichen voran.

```markdown
# Hauptüberschrift 1

Text

## Überschrift 2

Absatz 1

Absatz 2

### Überschrift 3

Text

* Erste Aufzählung
* Zweite Aufzählung

# Hauptüberschrift 2

.
.
.
```

Die Überschriften unterteilen Ihren Kurs in Seiten. Durch diese können Sie in der Vorschau (**Alt$+$L**) bzw. im Browser (**Strg$+$N**) entweder mit einem Klick auf die jeweilige Überschrift im Inhaltsverzeichnis oder mit den Pfeiltasten oben neben der Seitenzahl navigieren. Für eine aktuelle Vorschau speichern Sie Ihre Datei (**Strg$+$S**). Die Preview wird daraufhin automatisch aktualisiert.

<br>
$^* $Sollte sich keine ReadMe-Datei im Projektbaum innerhalb Ihres Projektordners auffinden lassen, können Sie diese in Atom unter File -> New File selbst erstellen.

$^{**} $Die Inhalte der Vorlagen können Sie kopieren und in Ihre Textdatei einfügen.


## **Einbinden von Medien**

Auf den folgenden Seiten finden Sie Möglichkeiten, Bilder, Videos oder Links in Ihren Kurs einzubinden.

### Bilder

Um ein Bild einzubinden, gibt es verschiedene Möglichkeiten.

~~Bilder aus dem **Projektordner**~~

Ein Bild, das sich in Ihrem Projektordner (also lokal auf ihrem Rechner bzw. online bei GitHub) befindet, binden Sie mittels URL ein. Nutzen Sie dazu folgende Vorlage:

`![image](image-url)`

Für das Finden der URL, öffnen Sie Ihren Kurs auf [GitHub](https://github.com) und dort den jeweiligen Ordner, in dem sich Ihr Bild befindet. Nach Anklicken des Bildes erscheint ihr Bild in einer Voranzeige. Im Kontextmenü des Bildes (rechte Maustaste) wählen Sie *Grafikadresse kopieren*. Diese fügen Sie in die runden Klammern ein.

`![image](https://raw.githubusercontent.com/ILIFV-NB/TestKurs/master/ErstesKursFoto.png)`

In der Preview (**Alt$+$L**) bzw. im Browser (**Strg$+$N**) erscheint an dieser Stelle Ihr Foto.

<br/>
~~Bilder aus dem **Internet**~~

Sie können aber auch ein Foto aus dem Internet einbinden.

Dazu öffnen Sie das gewünschte Foto im Internet, kopieren die Adresszeile und platzieren diese in den runden Klammern.

`![image](https://cdn.pixabay.com/photo/2019/11/02/21/45/maple-leaf-4597501_1280.jpg)`

![image](https://cdn.pixabay.com/photo/2019/11/02/21/45/maple-leaf-4597501_1280.jpg)<!--
style = "width: 80%; "
-->

Um Ihr Foto mit einem Rahmen (border) zu versehen oder die Größe (width) anzupassen, ergänzen Sie den Pfad durch entsprechende Angaben ...

`![image](https://cdn.pixabay.com/photo/2019/11/02/21/45/maple-leaf-4597501_1280.jpg)<!--`
<br/>
`style = "border: 1px solid; width: 80%; "`
<br/>
`-->`

... oder schauen sich [hier](https://liascript.github.io/course/?https://raw.githubusercontent.com/liaScript/docs/master/README.md#1) nach weiteren Inspirationen um.


### Videos

Um ein Video einzubinden, gibt es verschiedene Möglichkeiten.

~~Videos aus dem **Projektordner**~~

Ein Video, das sich in Ihrem Projektordner (also lokal auf ihrem Rechner bzw. online bei GitHub) befindet, binden Sie mittels URL ein. Nutzen Sie dazu folgende Vorlage:

`!?[movie](movie-url)`

Für das Finden der URL, öffnen Sie Ihren Kurs auf [GitHub](https://github.com) und dort den jeweiligen Ordner, in dem sich Ihr Video befindet. Nach Anklicken des Videos erscheint die Möglichkeit *View raw*. Die nun erscheinende Adresszeile kopieren Sie und fügen Sie in die runden Klammern ein. Um die Größe des Videos anzupassen, ergänzen Sie den Pfad wie folgt:

`!?[movie](https://raw.githubusercontent.com/ILIFV-NB/TestKurs/master/movies/math.mp4)<!--`
<br/>
`style = "height: 446px; width: 793px; "`
<br/>
`-->`

In der Preview (**Alt$+$L**) bzw. im Browser (**Strg$+$N**) erscheint an dieser Stelle Ihr Video.

<br/>
~~Videos aus dem **Internet** (YouTube)~~

Sie können aber auch ein Video aus dem Internet (z.B. YouTube) einbinden.

Dazu öffnen Sie das gewünschte Video auf YouTube, klicken mit der rechten Maustaste darauf und wählen ~~Einbettungscode kopieren~~. Diesen platzieren Sie an entsprechender Stelle in ihrem Dokument. Der Code beinhaltet bereits Größenangaben des anzuzeigenden Videos. Diese können Sie gern anpassen.

`<iframe width="793" height="446" src="https://www.youtube.com/embed/bICfKRyKTwE" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>`

<iframe width="533" height="300" src="https://www.youtube.com/embed/bICfKRyKTwE" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


### Links

Um einen Link zu vermerken, kopieren Sie diesen aus der Eingabezeile Ihres Browsers an die entsprechende Stelle in Ihrem Dokument.

https://liascript.github.io/

---------

Sie können diesen Link auch hinter einem Namen verstecken. Geben Sie dazu in Atom das Wort ~~link~~ ein und betätigen Sie die Tab-Taste. Es erscheint eine Vorlage:

`[name](url)`

Diese ergänzen Sie durch den von Ihnen gewählten Namen und die URL:

`[LIA](https://liascript.github.io/)`

Auf Ihrer Seite erscheint lediglich der Name:

[LIA](https://liascript.github.io/)


---------
Möchten Sie innerhalb Ihres Kurses auf eine andere Seite verweisen, nutzen Sie dazu die jeweilige Seitennummer. Diese befindet sich oberhalb einer jeden Seite. Gehen Sie wie oben beschrieben vor. Geben Sie anstelle der URL die Seitenzahl ein und stellen sie ihr eine # voran:

`[Einbinden von Medien](#7)`

[Einbinden von Medien](#7)


## **Visualisieren von Messdaten**

Nachfolgend finden Sie einige Möglichkeiten, Messdaten aus Textdateien (wie z.B. aus Rauheits- oder Kraftmessungen) in Form von Diagrammen zu visualisieren. [Hier](#26) gibt es eine kleine Anleitung für das Einbinden in Ihren Kurs (Punkt 4).


## **-> Beispiel**

In den [Vorlagen-Tabellen](#13) auf den folgenden Seiten befinden sich Beispieldaten zur Veranschaulichung der jeweiligen Visualisierung. Diese Daten ersetzen Sie ganz einfach durch Ihre Daten, indem Sie die Beispieldaten löschen ...

![image](https://raw.githubusercontent.com/ILIFV-NB/Leitfaden-Dozenten/master/images/Eingabefeld-Kraftverlauf.png)<!--
style = "width: 100%; "
-->

...  und Ihre Daten hineinkopieren.

![image](https://raw.githubusercontent.com/ILIFV-NB/Leitfaden-Dozenten/master/images/Textdatei-Kraftverlauf.png)<!--
style = "width: 100%; "
-->

Ein Klick auf den Pfeil unten links macht aus Ihren Daten ein Diagramm. Dieses können Sie als Bilddatei herunterladen (Pfeilsymbol oben rechts) und speichern. Um einzelne Graphen auszublenden, klicken Sie auf das jeweilige Symbol in der Legende.

![image](https://raw.githubusercontent.com/ILIFV-NB/Leitfaden-Dozenten/master/images/Diagramm-Kraftverlauf.png)<!--
style = "width: 100%; "
-->

Wenn Sie weitere Daten einlesen möchten, löschen Sie die vorherigen Daten aus dem Eingabefeld, kopieren Ihre neuen Daten hinein und führen die Visualisierung wie oben beschrieben durch. Rechts unter dem Eingabefeld befinden sich Pfeile, mit Hilfe derer sie zu allen eingegebenen Daten navigieren können. Für die neue Visualisierung ist jeweils ein Klick auf den blauen Pfeil links unter dem Eingabefeld notwendig.

## **-> Vorlagen**

* [Zerspankräfte Drehen](#14)<br/>
* [Rauheitskenngrößen](#15)<br/>
* [Rauheitsprofile](#16)<br/>
* [Durchmesser](#17)

### Zerspankräfte Drehen

``` cvs (Zeit in s - Kraft Fx in N - Kraft Fy in N - Kraft Fz in N)
0;1,5;2,4;0,2
1;1,8;2,1;0,5
2;1,1;2,9;0,8
3;1,1;2,9;-0,8
```
<script>

let data = `@input`.replace(/,/g, ".");

let split = data.match(/\d+(?:\.\d+)?|\-\d+(?:\.\d+)?/g);
//document.write(split);
let T = []
let Fx = []
let Fy = []
let Fz = []

for(let i=0; i<split.length; i=i+4) {
  T.push(parseFloat(split[i]));
  Fx.push(parseFloat(split[i+1]));
  Fy.push(parseFloat(split[i+2]));
  Fz.push(parseFloat(split[i+3]));
}

plotData(T, Fx, Fy, Fz);

function plotData(t, x, y, z) {

  let main = document.getElementById('main');
  main.hidden = false;

  let fx = []
  let fy = []
  let fz = []

  for(let i=0; i<t.length; i++) {
    fx.push([t[i], x[i]])
    fy.push([t[i], y[i]])
    fz.push([t[i], z[i]])
  }

  let chart = echarts.init(main);

  let option = {

    title : {
      display: false,
      text: "Zerspankraft",
      subtext: 'Drehen',
      itemGap: 10,
      textAlign: 'auto',
      textVerticalAlign: 'middle',
      textStyle: {
        fontSize: 30,
      },
      subtextStyle: {
        fontSize: 20,
      },
    },

    grid: {
      top: 120,
    },

    legend: {
        data:['Fx', 'Fy', 'Fz'],
        top: 80,
        itemGap: 30,
        itemWidth: 50,
        itemHeight: 20,
        textStyle: {
          fontSize: 24,
        },
    },

    toolbox: {
      show : true,
      feature : {
        mark : {show: true},
        dataZoom : {show: true},
        dataView : {show: true, readOnly: false},
        restore : {show: true},
        saveAsImage : {
          show: true,
          pixelRatio: 4,
        },
      },
    },

    xAxis: [{
      type: 'value',
      name: 'Zeit in s',
      nameLocation: 'middle',
      nameGap: 40,
      axisLabel: {
        fontSize: 20,
      },
      nameTextStyle: {
        fontSize: 20,
      },
    }],

    yAxis: [{
      type : 'value',
      name: 'Kraft in N',
      nameLocation: 'middle',
      nameGap: 60,
      axisLabel: {
        fontSize: 20,
      },
      nameTextStyle: {
        fontSize: 20,
      },
    }],


    series : [{
      name:'Fx',
      type:'line',
      data: fx,
      symbol: 'none',
      lineStyle: {
        width: 3,
      },
    },
    {
      name:'Fy',
      type:'line',
      data: fy,
      symbol: 'none',
      lineStyle: {
        width: 3,
      },
    },
    {
      name:'Fz',
      type:'line',
      data: fz,
      symbol: 'none',
      lineStyle: {
        width: 3,
      },
    }]
  };

  // use configuration item and data specified to show chart
  chart.setOption(option);

  window.addEventListener('resize', chart.resize);
}
</script>


<div id="main" style="position:relative; width:100%; height:600%;" hidden="true"></div>


### Rauheitskenngrößen

``` cvs (Messung - Ra in µm - Rz in µm - Rmax in µm)
1 0,5;2,1;2,5
2;0,8;3,0;3,3
3;0,6;2,5;2,9
```
<script>
let data1 = `@input`.replace(/,/g, ".");

let split1 = data1.match(/\d+(?:\.\d+)?|\-\d+(?:\.\d+)?/g);
//document.write(split1);
let M = []
let Ra = []
let Rz = []
let Rmax = []

for(let i=0; i<split1.length; i=i+4) {
  M.push(parseFloat(split1[i]));
  Ra.push(parseFloat(split1[i+1]));
  Rz.push(parseFloat(split1[i+2]));
  Rmax.push(parseFloat(split1[i+3]));
};

plotData(M, Ra, Rz, Rmax);

function plotData(t1, x1, y1, z1) {

  let main1 = document.getElementById('main1');
  main1.hidden = false;

  let ra = []
  let rz = []
  let rmax = []

  for(let i=0; i<t1.length; i++) {
    ra.push([t1[i], x1[i]])
    rz.push([t1[i], y1[i]])
    rmax.push([t1[i], z1[i]])
  }

  let chart1 = echarts.init(main1);

  let option1 = {

    title : {
      display: false,
      text: "Rauheit",
      subtext: 'Kenngrößen',
      itemGap: 10,
      textAlign: 'auto',
      textVerticalAlign: 'middle',
      textStyle: {
        fontSize: 30,
      },
      subtextStyle: {
        fontSize: 20,
      },
    },

    grid: {
      top: 120,
    },

    legend: {
        data:['Ra', 'Rz', 'Rmax'],
        top: 80,
        itemGap: 40,
        itemWidth: 50,
        itemHeight: 20,
        textStyle: {
          fontSize: 24,
        },
    },

    toolbox: {
      show : true,
      feature : {
        mark : {show: true},
        dataZoom : {show: true},
        dataView : {show: true, readOnly: false},
        restore : {show: true},
        saveAsImage : {
          show: true,
          pixelRatio: 4,
        },
      },
    },

    xAxis: [{
      type: 'category',
      nameLocation: 'middle',
      nameGap: 30,
      axisLabel: {
        fontSize: 20,
        formatter: 'Messung {value}'
      },
      nameTextStyle: {
        fontSize: 20,
      },
    }],

    yAxis: [{
      type : 'value',
      name: 'Rauheit in µm',
      nameLocation: 'middle',
      nameGap: 60,
      axisLabel: {
        fontSize: 20,
      },
      nameTextStyle: {
        fontSize: 20,
      },
    }],

    series : [
    {
      name:'Ra',
      type:'bar',
      data: ra,
      label: {
        show: true,
        rotate: 90,
        formatter: ra,
        fontSize: 18,
      },
    },
    {
      name:'Rz',
      type:'bar',
      data: rz,
      label: {
        show: true,
        rotate: 90,
        formatter: rz,
        fontSize: 18,
      },
    },
    {
      name:'Rmax',
      type:'bar',
      data: rmax,
      label: {
        show: true,
        rotate: 90,
        formatter: rmax,
        fontSize: 18,
      },
    }
    ]
  };

  // use configuration item and data specified to show chart
  chart1.setOption(option1);

  window.addEventListener('resize', chart1.resize);
}
</script>


<div id="main1" style="position: relative; width:100%; height:600%;" hidden="true"></div>


### Rauheitsprofile

<!--
style="font-size: 30px; margin: 0 0;"
-->
**P-Profil**


``` cvs (Taststrecke in µm - P-Profil in µm)
0,00  -2,500
400,00  -6,500
800,00  8,500
1200,00 4,500
1600,00 18,500
2000,00 14,500
2400,00 18,500
2800,00 4,500
3200,00 8,500
3600,00 -6,500
4000,00 -2,500
4400,00 -16,500
4800,00 -12,500
```
<script>
let data2 = `@input`.replace(/,/g, ".");

let split2 = data2.match(/\d+(?:\.\d+)?|\-\d+(?:\.\d+)?/g);
//document.write(split2);
let Lt = []
let P = []


for(let i=0; i<split2.length; i=i+2) {
  Lt.push(parseFloat(split2[i]));
  P.push(parseFloat(split2[i+1]));
};

plotData(Lt, P);

function plotData(t2, x2) {

  let main2 = document.getElementById('main2');
  main2.hidden = false;

  let p = []

  for(let i=0; i<t2.length; i++) {
    p.push([t2[i], x2[i]])
  }

  let chart2 = echarts.init(main2);

  let option2 = {

    title : {
      display: false,
      text: "Primärprofil",
      subtext: 'P-Profil',
      itemGap: 10,
      textAlign: 'auto',
      textVerticalAlign: 'middle',
      textStyle: {
        fontSize: 30,
      },
      subtextStyle: {
        fontSize: 20,
      },
    },

    grid: {
      top: 120,
    },

    legend: {
        data:['P-Profil'],
        top: 80,
        itemGap: 40,
        itemWidth: 50,
        itemHeight: 20,
        textStyle: {
          fontSize: 24,
          color: 'black',
        },
    },

    toolbox: {
      show : true,
      feature : {
        mark : {show: true},
        dataZoom : {show: true},
        dataView : {show: true, readOnly: false},
        restore : {show: true},
        saveAsImage : {
          show: true,
          pixelRatio: 4,
        },
      },
    },

    xAxis: [{
      type: 'value',
      name: 'Taststrecke in µm',
      nameLocation: 'middle',
      nameGap: 40,
      min: 0,
      max: 4800,
      interval: 800,
      axisLabel: {
        fontSize: 20,
      },
      nameTextStyle: {
        fontSize: 20,
      },
    }],

    yAxis: [{
      type : 'value',
      name: 'Profil in µm',
      nameLocation: 'middle',
      nameGap: 60,
      axisLabel: {
        fontSize: 20,
      },
      nameTextStyle: {
        fontSize: 20,
      },
    }],

    series : [
    {
      name:'P-Profil',
      type:'line',
      data: p,
      symbol: 'none',
      color: 'black',
      lineStyle: {
        width: 1,
        color: 'black',
      },
    },
    ]
  };

  // use configuration item and data specified to show chart
  chart2.setOption(option2);

  window.addEventListener('resize', chart2.resize);
}
</script>

<div id="main2" style="position: relative; width:100%; height:600%;" hidden="true"></div>

<br/>

<!--
style="font-size: 30px; margin: 0 0;"
-->
**R-Profil**


``` cvs (Messstrecke in µm - R-Profil in µm)
400,00  -2,500
800,00  2,500
1200,00 -2,500
1600,00 2,500
2000,00 -2,500
2400,00 2,500
2800,00 -2,500
3200,00 2,500
3600,00 -2,500
4000,00 2,500
4400,00 -2,500
```
<script>
let data3 = `@input`.replace(/,/g, ".");

let split3 = data3.match(/\d+(?:\.\d+)?|\-\d+(?:\.\d+)?/g);
//document.write(split3);
let Ln = []
let R = []


for(let i=0; i<split3.length; i=i+2) {
  Ln.push(parseFloat(split3[i]));
  R.push(parseFloat(split3[i+1]));
};

plotData(Ln, R);

function plotData(t3, x3) {

  let main3 = document.getElementById('main3');
  main3.hidden = false;

  let r = []

  for(let i=0; i<t3.length; i++) {
    r.push([t3[i], x3[i]])
  }

  let chart3 = echarts.init(main3);

  let option3 = {

    title : {
      display: false,
      text: "Rauheitsprofil",
      subtext: 'R-Profil',
      itemGap: 10,
      textAlign: 'auto',
      textVerticalAlign: 'middle',
      textStyle: {
        fontSize: 30,
      },
      subtextStyle: {
        fontSize: 20,
      },
    },

    grid: {
      top: 120,
    },

    legend: {
        data:['R-Profil'],
        top: 80,
        itemGap: 40,
        itemWidth: 50,
        itemHeight: 20,
        textStyle: {
          fontSize: 24,
        },
    },

    toolbox: {
      show : true,
      feature : {
        mark : {show: true},
        dataZoom : {show: true},
        dataView : {show: true, readOnly: false},
        restore : {show: true},
        saveAsImage : {
          show: true,
          pixelRatio: 4,
        },
      },
    },

    xAxis: [{
      type: 'value',
      name: 'Messstrecke in µm',
      nameLocation: 'middle',
      nameGap: 40,
      min: 0,
      max: 4800,
      interval: 800,
      axisLabel: {
        fontSize: 20,
      },
      nameTextStyle: {
        fontSize: 20,
      },
    }],

    yAxis: [{
      type : 'value',
      name: 'Profil in µm',
      nameLocation: 'middle',
      nameGap: 60,
      axisLabel: {
        fontSize: 20,
      },
      nameTextStyle: {
        fontSize: 20,
      },
    }],

    series : [
    {
      name:'R-Profil',
      type:'line',
      data: r,
      symbol: 'none',
      lineStyle: {
        width: 1,
      },
    },
    ]
  };

  // use configuration item and data specified to show chart
  chart3.setOption(option3);

  window.addEventListener('resize', chart3.resize);
}
</script>

<div id="main3" style="position: relative; width:100%; height:600%;" hidden="true"></div>

<br/>

<!--
style="font-size: 30px; margin: 0 0;"
-->
**W-Profil**


``` cvs (Messstrecke in µm - W-Profil in µm)
400,00  -2,000
800,00  6,000
1200,00 12,000
1600,00 16,000
2000,00 18,000
2400,00 18,000
2800,00 16,000
3200,00 12,000
3600,00 6,000
4000,00 -2,000
4400,00 -12,000
```
<script>
let data4 = `@input`.replace(/,/g, ".");

let split4 = data4.match(/\d+(?:\.\d+)?|\-\d+(?:\.\d+)?/g);
//document.write(split4);
let Ln1 = []
let W = []


for(let i=0; i<split4.length; i=i+2) {
  Ln1.push(parseFloat(split4[i]));
  W.push(parseFloat(split4[i+1]));
};

plotData(Ln1, W);

function plotData(t4, x4) {

  let main4 = document.getElementById('main4');
  main4.hidden = false;

  let w = []

  for(let i=0; i<t4.length; i++) {
    w.push([t4[i], x4[i]])
  }

  let chart4 = echarts.init(main4);

  let option4 = {

    title : {
      display: false,
      text: "Welligkeitsprofil",
      subtext: 'W-Profil',
      itemGap: 10,
      textAlign: 'auto',
      textVerticalAlign: 'middle',
      textStyle: {
        fontSize: 30,
      },
      subtextStyle: {
        fontSize: 20,
      },
    },

    grid: {
      top: 120,
    },

    legend: {
        data:['W-Profil'],
        top: 80,
        itemGap: 40,
        itemWidth: 50,
        itemHeight: 20,
        textStyle: {
          fontSize: 24,
        },
    },

    toolbox: {
      show : true,
      feature : {
        mark : {show: true},
        dataZoom : {show: true},
        dataView : {show: true, readOnly: false},
        restore : {show: true},
        saveAsImage : {
          show: true,
          pixelRatio: 4,
        },
      },
    },

    xAxis: [{
      type: 'value',
      name: 'Messstrecke in µm',
      nameLocation: 'middle',
      nameGap: 40,
      min: 0,
      max: 4800,
      interval: 800,
      axisLabel: {
        fontSize: 20,
      },
      nameTextStyle: {
        fontSize: 20,
      },
    }],

    yAxis: [{
      type : 'value',
      name: 'Profil in µm',
      nameLocation: 'middle',
      nameGap: 60,
      axisLabel: {
        fontSize: 20,
      },
      nameTextStyle: {
        fontSize: 20,
      },
    }],

    series : [
    {
      name:'W-Profil',
      type:'line',
      data: w,
      symbol: 'none',
      lineStyle: {
        width: 1,
      },
    },
    ]
  };

  // use configuration item and data specified to show chart
  chart4.setOption(option4);

  window.addEventListener('resize', chart4.resize);
}
</script>

<div id="main4" style="position: relative; width:100%; height:600%;" hidden="true"></div>


### Durchmesser


``` cvs (Messung - Ød in mm)
1;80,550
2;80,450
3;80,250
```
<script>
let data5 = `@input`.replace(/,/g, ".");

let split5 = data5.match(/\d+(?:\.\d+)?|\-\d+(?:\.\d+)?/g);
//document.write(split5);
let M1 = []
let D = []

for(let i=0; i<split5.length; i=i+2) {
  M1.push(parseFloat(split5[i]));
  D.push(parseFloat(split5[i+1]));
};

plotData(M1, D);

function plotData(t5, x5) {

  let main5 = document.getElementById('main5');
  main5.hidden = false;

  let d = []

  for(let i=0; i<t5.length; i++) {
    d.push([t5[i], x5[i]])
  }

  let chart5 = echarts.init(main5);

  let option5 = {

    title : {
      display: false,
      text: "Durchmesser",
      subtext: 'Welle/Passsitz',
      itemGap: 10,
      textAlign: 'auto',
      textVerticalAlign: 'middle',
      textStyle: {
        fontSize: 30,
      },
      subtextStyle: {
        fontSize: 20,
      },
    },

    grid: {
      top: 120,
    },

    legend: {
        data:['Durchmesser'],
        top: 80,
        itemGap: 40,
        itemWidth: 50,
        itemHeight: 20,
        textStyle: {
          fontSize: 24,
        },
    },

    toolbox: {
      show : true,
      feature : {
        mark : {show: true},
        dataZoom : {show: true},
        dataView : {show: true, readOnly: false},
        restore : {show: true},
        saveAsImage : {
          show: true,
          pixelRatio: 4,
        },
      },
    },

    xAxis: [{
      type: 'category',
      nameLocation: 'middle',
      nameGap: 30,
      axisLabel: {
        fontSize: 20,
        formatter: 'Messung {value}'
      },
      nameTextStyle: {
        fontSize: 20,
      },
    }],

    yAxis: [{
      type : 'value',
      name: 'Messwert in mm',
      nameLocation: 'middle',
      nameGap: 60,
      axisLabel: {
        fontSize: 20,
      },
      nameTextStyle: {
        fontSize: 20,
      },
    }],

    series : [
    {
      name:'Durchmesser',
      type:'bar',
      data: d,
      label: {
        show: true,
        rotate: 90,
        formatter: d,
        fontSize: 18,
      },
    },
    ]
  };

  // use configuration item and data specified to show chart
  chart5.setOption(option5);

  window.addEventListener('resize', chart5.resize);
}
</script>


<div id="main5" style="position: relative; width:100%; height:600%;" hidden="true"></div>

## **-> Hinweise**

* Für das Einbinden obiger Tabellen in ihren Kurs, benötigen Sie einen längeren Code, den sie aus der Textdatei für diese Online-Hilfe, in der Sie sich befinden, kopieren können. Die Vorgehensweise schauen Sie sich bitte unter [*FAQ -> LIA-Script -> 4. Textdateien visualisieren*](#26) an.

* Betätigen der Funktionstaste F5 aktualisiert die Seite und lässt alle Diagramme verschwinden. Ein erneuter Klick auf den blauen Pfeil unter dem Eingabefeld erzeugt ein neues Diagramm.
* Um sich einen Ausschnitt im Diagramm näher anzuschauen, klicken Sie über dem Diagramm auf das Zoom-Icon und wählen den zu betrachtenden Bereich im Diagramm aus. Den Ausgangszustand erhalten Sie mit Zoom-Reset.
* Wenn Sie erfahren möchten, welche Daten das aktuelle Diagramm beinhaltet, klicken Sie auf das Icon in Form eines Dokumentes.


## **Online stellen/aktualisieren**

Während Sie Ihre Kurse in Atom bearbeiten und die Voransicht (Strg$+$L) durch Speichern (Strg$+$S) aktualisieren, bleibt diese Version lediglich lokal. Um sie auch online zugänglich zu machen, müssen Sie Ihr Dokument zu GitHub hochladen.

Am Fuß der Software Atom finden Sie eine Beschriftung namens **Git**. Wenn Sie darauf klicken, öffnet sich rechts neben Ihrer Voransicht ein Bereich, in dessen oberem Teil sie Elemente sehen, die verändert wurden. Das wird in jedem Fall die ReadMe-Datei sein sowie ggf. hinzugefügte oder entfernte Fotos oder Videos. Sobald Sie die Änderungen online einpflegen möchten, klicken Sie auf **Stage All**. Die Elemente wandern in den unteren Teil der Ansicht und sind somit bereit, veröffentlicht zu werden.

Hierzu geben Sie in das Feld mit dem Inhalt 'Commit message' einen Hinweis ein, der etwas über die getätigten Änderungen aussagt (z.B. "Kapitel 3 eingefügt" oder "Fotos ergänzt") und bestätigen mit **Commit to master**.

Wiederum am unteren Rand der Software erscheint der Hinweis **push 1**. Mit einem Klick darauf öffnet sich ein Fenster, in das Sie Ihre GitHub LogIn-Daten* eintragen. Nun senden Sie die aktuelle Version Ihres Kurses zu GitHub, welche Sie wenige Sekunden später dort auffinden.

Alternativ sind Änderungen direkt in GitHub möglich. Um diese Änderungen in Atom (lokal) zu übernehmen, klicken Sie unten rechts auf **fetch**. Ihre Daten werden von GitHub abgerufen. Wenn Sie Ihren Kurs gemeinschaftlich bearbeiten, sollten Sie diesen Schritt stets durchführen, bevor Sie sich erneut Ihrem Kurs widmen. So entgehen Ihnen keinen Änderungen

<br/>
<!--
style="font-Size: 13px"
-->
$^* $ Um Ihre LogIn-Daten zu GitHub zu speichern, klicken Sie in Atom unten rechts auf das Katzensymbol (GitHub), folgen dem Link und generieren mit dem Einloggen ein Token, das Sie wiederum in Atom eingeben. Ab sofort genügt ein Klick auf **push**, um Ihren Kurs bei GitHub zu aktualisieren!


# ~~**Schnelleinstieg eLab**~~

Hier finden Sie eine kurze Einweisung in den Umgang mit der Webumgebung eLab. Dies betrifft u.a. den Zugang zur Webumgebung, das Einbinden von Kursen sowie das Einsehen von Teilnehmern und den Stand derer Kurse.

## Registrierung

Um Zugang zur Webumgebung eLab zu erhalten, registrieren Sie sich bitte zunächst auf folgender Website: [Webumgebung eLab](https://elab-hsmd-qa.dev.enterprises/).

<br>
![image](https://raw.githubusercontent.com/ILIFV-NB/Leitfaden-Dozenten/master/images/Register.jpg)<!--
style = "width: 100%;
        border: 1px solid; "
-->

Hier klicken Sie rechts oben auf *Register* und geben in der folgenden Maske Ihre Nutzerdaten ein. Mit einem Klick auf *Submit* sind Sie als User gespeichert. In dieser Rolle können Sie sich bereits eingepflegte Kurse ansehen. Um eigene Kurse einzubinden, benötigen Sie einen Zugang als Administrator. Wenden Sie sich hierzu bitte an [Nancy Brinkmann](#28) oder [Ronny Stolze](#28).

<br>
![image](https://raw.githubusercontent.com/ILIFV-NB/Leitfaden-Dozenten/master/images/Register-User.png)<!--
style = "width: 100%;
        border: 1px solid; "
-->

## Einbinden von Kursen

Um einen neuen Kurs anzulegen, klicken Sie im Menü auf ~~eLab~~ und dort auf den Button ~~New Course~~. Tragen Sie hier die notwendigen Informationen (inkl. URL$^* $) zu Ihrem Kurs ein und bestätigen Sie mit ~~Submit~~. Sobald Sie Ihren Kurs für die Studierenden zugänglich machen möchten, aktivieren Sie das Kontrollkästchen neben ~~Active~~. Einmal zugänglich, sollte ein Kurs nicht mehr verändert werden!!! (In diesen Bereich gelangen Sie wieder über *eLab -> jeweiliger Kurs ->  Edit*)

 $^* $ Die URL bekommen Sie auf [GitHub](https://github.com/). Öffnen Sie dort den jeweiligen Kurs und klicken Sie auf die ReadMe-Datei. Rechts erscheint ein Button mit dem Namen 'Raw'. Nachdem Sie diesen betätigt haben, landen Sie auf einer Seite mit den Rohdaten zu Ihrem Kurs. Der Inhalt in der Adresszeile ist die URL, die Sie für das Einpflegen in die Webumgebung eLab benötigen. Kopieren Sie diese und fügen Sie sie an entsprechender Stelle in der Webumgebung ein.


## Teilnehmereinsicht

Um die Liste der angemeldeten Teilnehmer einzusehen, sind Administratorrechte erforderlich. Wenden Sie sich hierzu bitte an [Nancy Brinkmann](#28) oder [Ronny Stolze](#28).

<br/>
~~Kurse der Teilnehmer als 'bestanden' markieren~~

Bis zu einer festgesetzten Frist hat der/die Studierende seine/ihre Arbeiten in den Kursen fertigzustellen. Gehen Sie nun im Menü auf ~~User~~ und schauen Sie sich jeweils mit einem Klick auf das Auge und anschließend auf ~~Course~~ den bearbeiteten Kurs an. Möchten Sie diesen als absolviert kennzeichnen, klicken Sie - wiederum unter User -> Auge - auf ~~Edit~~ des jeweiligen Kurses und setzen ein Häkchen (*accomplished*). Bitte Bestätigen Sie den Button ~~Submit~~ und senden dem/der Studierenden eine kurze Mail mit dem Vermerk, dass dieser sich nun für das Praktikum vor Ort eintragen kann. (*Eine andere Vorgehensweise ist derzeit technisch leider nicht möglich.*)

~~Teilnehmer de-/aktivieren~~

Wenn Sie einen Teilnehmer deaktivieren möchten, z.B., weil das Semester und die Abgabephase beendet sind, gehen Sie im Menü auf ~~User~~, klicken unter dem/der jeweiligen Studierenden auf den Bleistift und entfernen das Häkchen hinter ~~active~~.$ ^* $ Der Teilnehmer erhält nach dem nächsten Einloggen die folgende Nachricht:*Your Account has been deactivated, please contact your administrator*.

~~Teilnehmern eine bestimmte Rolle zuweisen~~

Gehen Sie im Menü auf ~~User~~, klicken unter dem/der jeweiligen TeilnehmerIn auf den Bleistift und ändern Sie hier neben ~~Role~~ den jeweiligen Status.$ ^* $

$ ^* $ Alternativ klicken Sie auf das Auge und oben rechts auf ~~Edit~~.

## Tickets einsehen

Wenn ein Studierender ein Problem in einem Kurs feststellt, kann er im Menü unter ~~Issues~~ ein 'Ticket' erstellen. Diese finden Sie, wenn Sie in einen beliebigen Kurs gehen, das Drop-Down Menü unter ~~Admin~~ wählen und dort ~~Tickets~~ anklicken. Mit ~~Edit~~ können Sie dem Text etwas hinzufügen und den Status ändern (*in progress, resolved, closed, etc.*). Diese Informationen sind ausschließlich vom Admin einzusehen.

# **FAQ**

Nachfolgend finden Sie einige allgemeine Hinweise zum Tool [LIA-Script](https://liascript.github.io/course/?https://raw.githubusercontent.com/liaScript/docs/master/README.md#1) bzw. zur [Webumgebung eLab](https://elab-hsmd-qa.dev.enterprises/).

## LIA-Script

`1.` Wie navigiere ich innerhalb der Preview in Atom?

|Aktion|Shortcut|
|---|---|
|Preview einblenden |Alt$+$L |
|Preview aktualisieren | Strg$+$S |
|Preview zurücksetzen$^*$ | Strg$+$S oder F5 |
|zurück | Alt$+$links |
|vor |Alt$+$rechts |
|zur Textstelle in ReadMe springen|Doppelklick in Preview|
|zur Textstelle in Preview springen|Doppelklick in ReadMe|

$^* $ nach Ausführen von Visualisierungen oder Beantworten von Quizzen etc.

<br>

`2.` Wie installiere ich die Plugins für Atom?

Nach Eingabe folgender Tastenkombination **Strg$+$Shift$+$P** geben Sie in die Suchleiste  ~~settings~~ ein und scrollen solange herunter bis *Settings View: Install Packages and Themes* erscheint. Hier geben Sie in die Suchleiste ~~liascript~~ ein. Es erscheinen aktuell zwei Plugins ([liascript-preview](https://atom.io/packages/liascript-preview) und [liascript-snippets](https://atom.io/packages/liascript-snippets)), die Sie installieren können. (Alternativ nutzen Sie die Links an dieser Stelle.) Wenn es Updates gibt, werden Sie innerhalb Atom darauf hingewiesen.

<br>

`3.` Was kann ich mit den Plugins anfangen?

Das Plugin **liascript-preview** bietet Ihnen bspw. die Möglichkeit, eine Voransicht Ihres Kurses, wie er im Browser erscheinen wird, anzusehen und auszuprobieren, ob Bilder und Videos so erscheinen, wie Sie das wünschen oder ob Links funktionieren.

Das Plugin **liascript-snippets** hilft Ihnen dabei, Befehle zur Erstellung von bspw. Links zu finden bzw. zur Einbindung von Medien. Dazu geben Sie im Editor  ~~lia~~ (oder den Suchbegriff) ein und es erscheinen einige Vorschläge.

<br>

`4.` Textdateien visualisieren

Um Tabellen wie unter [Visualisieren von Messdaten](#11) in Ihrem Kurs zu nutzen, können Sie der Textdatei für diese Online-Hilfe, in der Sie sich befinden, den dazugehörigen Code entnehmen. Gehen Sie oben in die Adresszeile Ihres Browsers und löschen alles, was vor 'https://raw.github[...]' steht. Nach einem Klick auf 'Enter' sehen Sie den Rohtext dieser Online-Hilfe. Mit Strg$+$F finden Sie die gesuchte Stelle im Dokument. Kopieren Sie sich den gewünschten Inhalt und fügen Ihn in Ihren Kurs ein.

Zusätzlich ist das Einfügen des folgenden Eintrags in den Header erforderlich:

`script:  https://cdnjs.cloudflare.com/ajax/libs/echarts/4.2.1/echarts-en.js`

Fügen Sie diesen am Ende nach Ihrem Kommentar ein.


## eLab

`1.` Vorgehensweise, wenn ein(e) Studierende(r) das Passwort vergessen hat.

Sie loggen sich in die [Lernumgebung eLab](https://elab-hsmd-qa.dev.enterprises/) ein, gehen im Menü auf ~~User~~, klicken unter dem/der jeweiligen Studierenden auf den Bleistift und geben in die Zeilen ~~Password~~ und ~~Password Confirmation~~ ein Einmalpasswort ein, das Sie dem Studierenden per E-Mail mitteilen - mit der Bitte, dieses zu ändern.

`2.` Teilnehmer deaktivieren

Wenn Sie einen Teilnehmer deaktivieren möchten, z.B., weil das Semester und die Abgabephase beendet sind, gehen Sie im Menü auf ~~User~~, klicken unter dem/der jeweiligen Studierenden auf den Bleistift und entfernen das Häkchen hinter ~~active~~. Der Teilnehmer erhält nach dem Einloggen die folgende Nachricht: *Your Account has been deactivated, please contact your administrator*.



# Kontakt

Nancy Brinkmann <br>
E-Mail: nancy.brinkmann(at)h2.de

Ronny Stolze <br>
E-Mail: ronny.stolze(at)h2.de
