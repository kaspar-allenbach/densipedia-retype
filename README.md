# Densipedia Neue Typografie

Die Densipedia website erhält eine neue Schrift.
Die Einbindung findet via Adobe Fonts mittels Fontlizenz von EspaceSuisse statt.

* Intro Screencast: https://capture.dropbox.com/aX4P5syZcZGl4PXj *

# Website anschauen

https://kaspar-allenbach.github.io/densipedia-retype/

# Code via Github Codespaces

1. Start Github Codespaces:
2. `./website serve`
3. Die site lässt sich so online anschauen

# Fake templates

Über die toplevel menubar kommt man auf die statischen Templates, welche die neue Schrift zeigen.
Der CSS Code wird vermutlich unbenutzbar sein, aber da kann man die Schriften rausmessen.

# Typografisches Konzept

Die Schriften kommen über den Adobe Font Service. EspaceSuisse hält dazu eine Adobe Liezenz
`<link rel="stylesheet" href="https://use.typekit.net/{{ adobeID }}.css" />`

## Schriftarten

Es gibt zwei Schriftarten. Die Lauftextschrift `--ff-txt` und die Displayschrift: `--ff-display`
Die Serifenschrift wird für Lauftexte, Zitate, Leads und alles verwendet was im Lesefluss ist.
Die Serifenlose wird verwendet für Titel, Navigationen, Cards, Header, Footer und alles drumherum

## Schriftgrössen

Es gibt 6 Schrifftgrössen.

```
--fs-XS
--fs-S
--fs-M
--fs-L
--fs-XL
--fs-XXL
```

Sämtliche Texte müssen einem dieser Grössen zugeordnet werden.

## Line Height & Font Weight

Die Line height wurde geändert und muss ebenfalls überall angewendet

```
--ff-line-txt: 1.4;
--ff-line-display: 1.1;
```

Da in der Schriften welt leider keine konsistente Werte für Schriftschnitte angewendet werden können muss für den Display schnitt denn wert 300 verwendet werden. Der html default wert `600` führt zu falschem Schriftbild

```
--ff-display-bold: 300;
--ff-txt-regular: 400;
```
