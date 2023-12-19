
## <span style="color: #9C68C8;">Bonus: Wie benutze ich Python auf meinem eigenen Computer?</span>

🚨 **<span style="color: #b30000;">Achtung:</span>** ***Die folgende Anleitung beinhaltet das Herunterladen von Inhalten aus dem Internet. Das Ausführen von Programmen, die von fremden Leuten geschrieben wurden, kann extrem gefährlich sein und kann deinen Computer beschädigen, deine Daten gefährden oder sogar alle Geräte, die mit deinem Netzwerk verbunden sind, gefährden. Das gilt für alle Software inklusive Programme, Bibliotheken oder fremden Code. Stelle also sicher, dass du weißt, was du tust und was du da gerade herunterlädst und habe am besten jemanden dabei, der schon einmal Python installiert hat. Du kannst zum Beispiel deinen Lehrer für diesen Kurs fragen!***

Wenn du Lust hast, nach diesem Kurs weiter mit Python zu arbeiten, dann kannst du diese Anleitung befolgen, um Python auf deinem Rechner laufen zu lassen. Diese Anleitung erhebt keinen Anspruch an Vollständigkeit und es kann sein, dass du zwischendurch auf Probleme stößt. Gehe dann am besten auf deine Lehrenden zu.

🔎 <span style="color: #2E88B6;"> Die unten stehenden Anleitungen sind sehr ausführlich. Für den Anfang empfehlen wir *Google Colab* oder *Python* mit *Spyder* zu verwenden. Alle weiteren Vorschläge sind eher dazu da, dass ihr wisst, was die möglichen nächsten Optionen wären!</span>

Wenn du Python nicht auf deinem Rechner installieren willst, aber trotzdem mit Python arbeiten möchtest, kannst du auch Online-Versionen von Python verwenden. Ein Beispiel für solch einen Service ist Google Colab https://colab.research.google.com/. Das ist nicht nur deutlich einfacher, sondern auch deutlich sicherer!

Die nächsten Schritte beinhalten die Installation von Python, IDEs (gleich dazu mehr), Bibliotheken und Jupyter Notebooks. Das ist relativ kompliziert, wenn du selber jeden Schritt einzeln durchführen musst. Wenn du das noch zu kompliziert findest, dann kannst du auch Anaconda (https://www.anaconda.com/download/) installieren. Das ist ein Programm, das Python, IDEs, Jupyter, und ein paar Bibliotheken bündelt und die Nutzung von Python deutlich zugänglicher macht.

Python läuft auf so gut wie jedes Betriebssystem und ist sehr einfach zu installieren. Gehe dazu einfach auf https://www.python.org/downloads/ und schaue nach der neuesten Version. Stelle dabei sicher, dass du eine Version von *Python 3* auswählst und nicht *Python 2*. Gehe dann einfach den ganz normalen Installationsprozess durch. Stelle dabei sicher, dass du die Option auswählst, Python zu PATH hinzuzufügen. Das vereinfacht dann später das Installieren von Bibliotheken. 

Wenn die Installation fehlerfrei gelaufen ist, dann solltet ihr jetzt Python in eurem Terminal nutzen können (*CMD* unter Windows). Öffnet eurer Terminal und gebt `ipython` ein. Ihr solltet dann eure aktuelle Python-Version, gefolgt von `In [1]:` sehen. Dort könnt ihr nun Python-Befehle eingeben. Das Ganze ist aber nicht sehr empfehlenswert. Alternativ könnt ihr euren Code in einem Texteditor schreiben, das Dokument mit der Endung `.py` speichern, und dann die Datei mit `python dateiname.py` im Terminal ausführen. Achte allerdings darauf, dass der Pfad zur Datei richtig sein muss. Das Ganze ist allerdings nicht ganz so benutzerfreundlich. Deswegen kommen wir jetzt zu IDEs.

#### <span style="color: #C26BCA;"> IDEs ('Integrated Development Environments')</span>
Eine IDE ('integrated development environment') ist ein Programm, welches dir das Coden deutlich vereinfacht. Im Grunde kann man jedes Programm zum Coden verwenden, welches Text bearbeiten kann. Allerdings vereinfacht ein IDE das Leben deutlich dadurch, dass es besondere Features hat. Zum Beispiel können die meisten IDEs Variablen, Funktionen, usw. erkennen und dir den Code so darstellen, dass es durch Farben deutlich besser zu lesen ist. Des Weiteren können IDEs auch noch einfache Fehler im Code (wie z.B. offene Klammern, die nie geschlossen wurden `print('Das ist ein Fehler'`) erkennen oder die Programme direkt ausführen. Manche IDEs können euch sogar mit Large Language Models wie ChatGPT unterstützen.

Im Grunde sind IDEs ganz von eurer Python-Installation unabhängig und spielen also für den Rest der Anleitung keine Rolle.

Python kommt mit einer sehr rudimentären IDE, die *IDLE* heißt. Anaconda kommt mit verschiedenen IDEs, wie zum Beispiel *Spyder*.

Es gibt sehr viele verschiedene IDEs auf dem Markt. Eine der meistgenutzten ist wohl *Visual Studio Code* von Microsoft (https://code.visualstudio.com/). Des Weiteren sind unter anderem PyCharm (https://www.jetbrains.com/pycharm/), Atom (https://atom-editor.cc/) und Spyder (https://www.spyder-ide.org/) sehr beliebt. Was genau man jetzt benutzt, spielt keine große Rolle und kommt letztendlich auf die persönliche Präferenz an. VS Code ist zum Beispiel besonders vielseitig dadurch, dass man die Funktionalität durch Erweiterungen anpassen kann, was das Ganze aber auch ein bisschen verwirrend machen kann. Spyder ist hingegen nicht so vielfältig, dafür aber besonders anfängerfreundlich. 

Für sehr fortgeschrittene Programmierer gibt es auch noch 'IDEs' für die Kommandozeile, wie zum Beispiel Neovim (https://neovim.io/). Wir würden davon aber für Anfänger stark abraten.

#### <span style="color: #C26BCA;"> Bibliotheken Installieren </span>

Um Bibliotheken zu installieren ist es wichtig, dass ihr Python als PATH variable definiert habt. Das ist leider von Betriebssystem zu Betriebssystem unterschiedlich. Um zu testen, ob das der Fall ist, könnt ihr eure Kommandozeile benutzen (auf Windows heißt diese *CMD* und auf Linux/macOS heißt diese *Terminal*). Je nach Installation könnt ihr nun einen der folgenden Befehle eingeben (wenn Ihr nicht sicher seid, dann könnt ihr auch alle 3 ausführen):`
 
`py --version`

`python --version`

`python3 --version`

Wenn ihr die Version von Python bei einem der Befehle seht, dann habt ihr alles richtig gemacht. Ansonsten könnt ihr jemanden aus unserem Team oder euren Lehrenden fragen oder dem Tutorial auf https://realpython.com/add-python-to-path/ folgen (***achtet bei Tutorials immer darauf, dass sie von seriösen Quellen kommen!***).

Wenn das jetzt erledigt ist, dann könnt ihr Bibliotheken ganz einfach mit dem Befehl `pip install` installieren. PIP steht für "Pip Installs Packages" und ist ein sogenanntes *Paket-Management-System*, das für euch Bibliotheken installieren kann. Wenn ihr zum Beispiel NumPy installieren wollt, dann könnt ihr den folgenden Befehl benutzen:

`pip install numpy`

Fast immer findet ihr in der Dokumentation von der Bibliothek einen Abschnitt zur Installation (für NumPy findet ihr diesen unter https://numpy.org/install/). Es ist nie verkehrt, diesen Abschnitt zu lesen, denn Bibliotheken sind von anderen Bibliotheken abhängig, die zuerst installiert werden müssen. Um die Bibliothek wieder zu entfernen, könnt ihr den Befehl `pip uninstall` gefolgt von dem Paketnamen benutzen.

Sollte der obige Python Befehl funktioniert haben, aber pip nicht, dann kann es sein, dass ihr stattdessen `pip3` verwenden muss. Alternativ könnt ihr den Befehl `python -m pip ...` versuchen, wobei anstelle von `python` auch `py` oder `python3` stehen kann. 

Solltet ihr Anaconda installiert haben, dann müsst ihr einen anderen Befehl benutzen. Anaconda hat nämlich ein eigenes Paket-Management-System. Für die Installation nutzt ihr den Befehl `conda install` und für die Entfernung `conda remove`.

Für fortgeschrittenere Schülerinnen empfehlen wir, dass ihr euch mit Virtual Environments beschäftigt. Diese ermöglichen es nämlich für jedes Projekt, eine unterschiedliche Sammlung an Bibliotheken zu verwenden, ohne dass potenzielle Konflikte entstehen.

#### <span style="color: #C26BCA;"> Jupyter Notebooks </span>

Für die Kurse nutzen wir ausschließlich Jupyter Notebooks. Standardmäßig benutzt man Textdokumente, die in `.py` enden, um Python-Code zu schreiben. Jeglicher Output erfolgt dann aber in einem separaten Fenster oder in der Kommandozeile. Jupyter Notebooks ermöglichen es aber, Text, Code und die Ausgaben zu kombinieren. Dadurch wird alles extrem übersichtlich, was Jupyter Notebooks besonders beliebt in *Data Science* machen. Die entsprechenden Dateien haben die Endung `.ipynb`. Python kann standardmäßig nicht mit Jupyter Notebooks arbeiten. Dazu müssen wir das Ganze wie folgt installieren:

`pip install notebook`

Alternativ gibt es auch noch Jupyter Lab, was ein bisschen vielfältiger ist:
`pip install jupyterlab`

Ihr könnt wie immer über beide Optionen in der Dokumentation nachlesen: https://docs.jupyter.org/en/latest/.
Um Jupyter zu verwenden, könnt ihr in das Terminal `jupyter notebook` oder `jupyter lab` eingeben, je nachdem, was ihr installiert habt. In eurem Browser sollte sich dann ein Fenster öffnen, in dem ihr das jeweilige Programm verwenden könnt.
Mit `jupyter notebook dateiname.ipynb` oder `jupyter lab dateiname.ipynb` könnt ihr dann auch die entsprechenden Dateien öffnen.
Die meisten IDEs können auch `.ipynb` Dateien öffnen. Wie genau man das ermöglicht, unterscheidet sich von IDE zu IDE.

