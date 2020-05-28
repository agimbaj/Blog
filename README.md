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

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/agimbaj/Blog/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
