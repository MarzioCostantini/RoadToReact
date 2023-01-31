##react-router-dom

ist eine Bibliothek für die Navigation in React-Anwendungen. Mit react-router-dom können Sie verschiedene Teile Ihrer Anwendung zu verschiedenen URLs verknüpfen, so dass Benutzer beim Klicken auf Links oder beim Eingeben von URLs innerhalb Ihrer Anwendung navigieren können.

install

```
npm i react-router-dom
```

Ein Beispiel für die Verwendung von react-router-dom sieht folgendermaßen aus:

```
import { BrowserRouter, Routes, Route } from 'react-router-dom';

    <BrowserRouter>
      <Routes>
        <Route path="/dashboard" element={< Dashboard />}/>
        <Route path="/kontakte" element={< Kontakte />}/>
        <Route path="/aufgaben" element={< Aufgaben />}/>
      </Routes>
    </BrowserRouter>
```
