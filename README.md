## Welcome to GitHub Pages

Willkommen bei meinem Blog. Ich berichte hier über meine Projekte, die ich in der Zeit in der GPB gemacht habe.


### Wikipedia Statistik

Das erste Projekt, was ich gemacht habe war eine Software, die überprüft wie viele Wörte in einem Wikipedia Artikel sind, diese werden dann ausgewertet und anhand eines Balkendiagrammes angezeigt. Außerdem kann der Benutzer nach einem Wort selber suchen und je nach Angabe des Wortes oder Buchstaben verändert sich auch das Balkendiagramm mit. Beim Codieren musste ich mich mit Regex, Linq und Xml auseinandersetzen.

```markdown
On _TextChanged Event

MatchCollection matches = Regex.Matches(richTextBox1.Text, textBoxKeyword.Text,
                                        RegexOptions.IgnoreCase);
            //richTextBox und textBoxKeyword werden überprüft

            if (textBoxKeyword.TextLength > 0)
            {
                foreach (Match match in matches)
                    //für jede Übereinstimmung
                {
                    if (!stopWords.Contains(match.Value))
                        //falls eine Übereinstimmung gefunden wurde
                    {
                        zaehler++;
                        richTextBox1.Select(match.Index, textBoxKeyword.TextLength);
                        richTextBox1.SelectionBackColor = Color.Yellow;
                        //das Wort wird gelb makiert und der Zähler erhöht
                    }
                }
            }
```
#### Grafische Benutzeroberfläche
![Form1 07 05 2020 11_25_31](https://user-images.githubusercontent.com/64414327/81278606-3476a780-9056-11ea-83a0-3bfc9dd26e15.png)

### Unity Lernen

Nachdem ich mit dem Projekt fertig war habe ich mich zum ersten Mal mit Unity auseinandergesetzt. Ich habe durch YouTube Videos bestimmte Dinge gelernt. Klicken Sie [hier](https://www.youtube.com/watch?v=DZbQRw-ftnU&list=PL_pqkvxZ6ho1g_e56fct7Cm6bgQBhmAqN) um auf die Playlist zu gelangen, die ich mir angeguckt habe und mitgeschrieben habe.

### Erstes Unity Projekt

Nachdem ich fertig mit dem Tutorial war habe ich beschlossen mein eigenes Projekt zu starten. Die Idee ist ein First Person 3D Adventure Game zu kreieren in dem der User die Welt erkundet und Items sammeln kann. Außerdem soll er mit einer Waffe Monster töten und Erfahrungspunkte sammeln.
Zur Zeit liegt mein Fortschritt bei ca 10%. Ich bin erst fertig mit dem Terrain und die Bewegung,Gravitation und Kamerabewegung des Players

#### Terrain
Das Terrain hat eine Gesamtgröße von 12000 x 12000 x 12000 und besteht aus Sand, Moos, Lava, Stein, Erde, Eis und Laubblätter Texturen

![Paintball - SampleScene - PC, Mac   Linux Standalone - Unity 2019 3 14f1 Personal  PREVIEW PACKAGES IN USE _ _DX11_ 27 05 2020 11_42_36 (2)](https://user-images.githubusercontent.com/64414327/83118782-1c32ff00-a0cf-11ea-8e74-2cdd64bc29fd.png)

#### Movement

```markdown
```
