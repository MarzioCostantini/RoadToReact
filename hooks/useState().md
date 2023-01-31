## useState

ist ein React Hook, der es Ihnen ermöglicht, den Zustand (state) Ihrer Komponente zu verwalten. Ein Zustand ist eine Art von Daten, die sich innerhalb Ihrer Komponente ändern können und beeinflussen, wie die Komponente gerendert wird.

Hier ist ein Beispiel für die Verwendung des useState Hooks:

```
import React, { useState } from 'react';

function Example() {
  // Deklariert eine neue Zustandsvariable "count"
  const [count, setCount] = useState(0);

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

In diesem Beispiel wird eine Zustandsvariable namens count mit dem Wert 0 initialisiert. Die useState-Funktion gibt ein Array mit zwei Elementen zurück: den aktuellen Wert des Zustands (count) und eine Funktion (setCount), mit der Sie den Zustand ändern können. In diesem Beispiel wird die setCount-Funktion bei jedem Klick auf den Button aufgerufen, um den Wert von count um 1 zu erhöhen.

Mit dem useState Hook können Sie den Zustand Ihrer Komponente verwalten, ohne dass Sie eine Klasse verwenden müssen. Stattdessen können Sie Ihre Komponente als Funktion schreiben, die einfacher zu lesen und zu verstehen ist.
