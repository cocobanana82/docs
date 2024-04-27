# Pfeil-Funktionen

**Beschreibung**: Pfeil-Funktions-Ausdrücke wurden in ES6 eingeführt. Diese Ausdrücke bieten eine saubere und prägnante Alternative zur traditionellen Funktionssyntax.

## Themenbereiche

- Webentwicklung
- Informatik

## Tags

- Argumente
- ES6
- Funktionen
- Parameter

## Kataloginhalt

- Einführung in JavaScript
- Karriereweg/Front-End-Ingenieur

**Pfeil-Funktions-Ausdrücke** sind Alternativen zu traditionellen [Funktionen](https://www.codecademy.com/resources/docs/javascript/functions), die erstmals in ES6 eingeführt wurden. Neben einer relativ prägnanten Syntax weisen Pfeil-Funktionen einige semantische Unterschiede sowie einige Einschränkungen auf.

## Syntax

```js
const functionA = (parameter1, parameter2, ..., parameterN) => {
  // Funktions Körper hier...
}
```

Die Syntax für einen Pfeil-Funktions-Ausdruck erfordert nicht das Schlüsselwort `function` und verwendet einen Fettpfeil (`=>`) um die Parameter vom Körper zu trennen.

Pfeil-Funktionen können mit null oder mehr Parametern definiert werden, auf einer oder mehreren Zeilen. In den meisten Fällen sind Klammern `()` um die Parameterliste nicht erforderlich, wenn es einen Parameter gibt. Sie sind erforderlich in den folgenden Fällen:

- Es gibt mehr als einen Parameter.
- Es gibt keine Parameter.
- Der einzelne Parameter ist ein destrukturiertes Objekt.
- Es sind Standard- oder Restparameter beteiligt.

Pfeil-Funktionen mit einem einzigen Ausdruck haben keine geschweiften Klammern (`{}`) und können den prägnanten Funktionskörper verwenden, um das Ergebnis des Ausdrucks ohne das Schlüsselwort `return` zurückzugeben. Bei mehreren Ausdrücken können Klammern alternativ um den Pfeilfunktionskörper gewickelt werden, um das Ergebnis implizit zurückzugeben.

## Einschränkungen

Pfeil-Funktionen sind begrenzt und können nicht in allen Situationen verwendet werden:

- Sie haben keine eigenen Bindungen an [`this`](https://www.codecademy.com/resources/docs/javascript/this) oder [`super`](https://www.codecademy.com/resources/docs/javascript/super) und sollten nicht als [Methoden](https://www.codecademy.com/resources/docs/javascript/methods) verwendet werden.
- Sie können nicht als [Konstruktoren](https://www.codecademy.com/resources/docs/javascript/constructors) verwendet werden.
- Sie können [`yield`](https://www.codecademy.com/resources/docs/javascript/yield) innerhalb ihres Körpers nicht verwenden.
- Sie können das spezielle Schlüsselwort [`arguments`](https://www.codecademy.com/resources/docs/javascript/arguments) nicht verwenden.

## Beispiel

Das folgende Beispiel zeigt, wie Pfeil-Funktionen definiert und angewendet werden:

```js
const printHello = () => { console.log('hallo'); };
const checkWeight = (gewicht) => { console.log(`Gepäckgewicht: ${gewicht} Kilogramm.`); };
printHello();
checkWeight(25);
```

Dies ergibt die folgende Ausgabe:

```shell
hallo
Gepäckgewicht: 25 Kilogramm.
```

## Codebyte-Beispiel

Das folgende Beispiel zeigt eine Pfeil-Funktion, die mit zwei Argumenten in einer einzigen Zeile definiert ist:

```js
const multiply = (a, b) => a * b;
console.log(multiply(2, 30));
```
