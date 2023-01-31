## useEffect

ist ein React Hook, der es Ihnen ermöglicht, nebenläufige Effekte (side effects) in Ihren Funktionskomponenten auszuführen. Effekte sind Aktionen, die Sie ausführen möchten, wenn sich eine bestimmte Änderung in Ihrer Komponente ergibt, wie z.B. das Laden von Daten aus einer API oder das Überwachen der Größe des Browserfensters.

Hier ist ein Beispiel für die Verwendung des useEffect Hooks:

```
import React, { useState, useEffect } from 'react';

function Example() {
  const [count, setCount] = useState(0);

  // Die "effect"-Funktion wird ausgeführt, wenn sich count ändert
  useEffect(() => {
    document.title = `You clicked ${count} times`;
  }, [count]);

  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>
        Click me
      </button>
    </div>
  );
}
```

In diesem Beispiel wird die useEffect-Funktion aufgerufen, wenn sich der Wert von count ändert. Die useEffect-Funktion ändert den Titel des Dokuments, um die Anzahl der Klicks anzuzeigen. Die zweite Argument von useEffect, ein Array von Abhängigkeiten, bestimmt, wann die useEffect-Funktion erneut ausgeführt werden soll. In diesem Fall wird die useEffect-Funktion jedes Mal ausgeführt, wenn sich count ändert.

Mit dem useEffect Hook können Sie nebenläufige Effekte in Ihren Funktionskomponenten ausführen, ohne dass Sie eine Klasse verwenden müssen. Außerdem können Sie durch die Angabe der Abhängigkeiten präzise bestimmen, wann die Effekte ausgeführt werden sollen, um die Leistung Ihrer Anwendung zu optimieren.
