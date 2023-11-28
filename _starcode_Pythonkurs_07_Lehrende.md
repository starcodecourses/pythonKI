# **<span style="color: #6162C5;">Künstliche Intelligenz mit Python</span>  <span style="color: #7865C6;"> - Notizen für Lehrende zu 'Woche 7: Einführung in das Maschinelle Lernen'</span>** 

In diesem Dokument finden Lehrende alle zusätzlichen Hinweise für die Unterrichtswoche 6. Man beachte, dass das hier bereitgestellte Material nicht unbedingt für die Unterrichtsstunden verwendet werden muss und zusätzliche Inhalte so gestaltet werden können, wie es zu dem Unterrichtsstil passt. 

Der wichtigste Teil des Kurses ist die Erklärung der Begriffe rund um das maschinelle Lernen! Sollte das training des NN zu lange brauchen, kann auch die Anzal der Neuronen in den 'Dense' Layern reduziert werden. Alternativ kann auch einer der beiden Layer entfernt werden!

## <span style="color: #9C68C8;">Wiederholungsquiz zur 6. Woche:</span>
*Frage 1:* Wie erhält man den Wert der an der 3. Zeile und 2. Spalte eines 2D-Arrays `array` steht?
- [ ] `array[2,3]`
- [ ] `array(3,2)`
- [ ] `array[3,2]`
- [x] `array[2,1]`

*Frage 2:* Was ist die Reihenfolge von den Werten in einem Slice?
- [x] `start:stop`
- [x] `start:stop:step`
- [ ] `step:start:stop`
- [ ] `start:step:stop`

*Frage 3:* Wie kann man NumPy Arrays Elementweise Teilen
- [x] `np.divide()`
- [x] `/`
- [ ] `np.div()`
- [ ] `÷`

*Frage 4:* Wie kann man sich die 5 ersten Zeilen eines Datensatzes `daten` mit Pandas anzeigen lassen?
- [ ] `daten.info(5)`
- [ ] `daten.first(5)`
- [x] `daten.head(5)`
- [ ] `daten.info(4)`

*Frage 5:* Wie kann man auf die 5 bis 8 Zeile eines Datensatzes `daten` mit Pandas zugreifen?
- [ ] `daten.locate[5:8]`
- [x] `daten.iloc[4:7]`
- [ ] `daten.loc[4:7]`
- [ ] `daten.iloc[5:8]`

*Frage 6:* Was ist der richtige Ausdruck, um alle Planeten im Datensatz `planeten` zu finden, die in der Spalte `Atmosphäre?` ein `Ja` stehen haben?
- [ ] `planeten['Atmosphäre?'=='Ja']`
- [x] `planeten.loc[planeten['Atmosphäre?']=='Ja']`
- [ ] `planeten[planeten['Atmosphäre?']=='Ja']`
- [ ] `planeten.iloc[planeten['Atmosphäre?']=='Ja']`
