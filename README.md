# Beispielanwendung zur Integration von Webkomponenten

1. Anlage einer `index.html` zur Integration der Webkomponenten
2. Webkomponent-Bundles werden über das `<script>`-Tag eingebunden.
   Beispiel:

```
 <script src="./angular/main.js"></script>
```

3. Properties können über Attribute in die Komponente hineingegeben werden

```
<vkb-input value="Eingabe"></vkb-input>
```

4. Komponenten können Customevents auslösen. Hier kann beispielsweise in der Appshell darauf reagiert werden.

```javascript
var hello = document.querySelector('vkb-input');
hello.addEventListener('valueChanged', function(e) {
  console.log(e.detail);
});
```
