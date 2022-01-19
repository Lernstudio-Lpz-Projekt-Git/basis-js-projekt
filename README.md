# basis-js-projekt

Bei diesem Repository handelt es sich um eine "Test-/Entwicklungsumgebung" die auf Gulp, TypeScript/JS, ES6+ und Sass basiert.

# IDE 11/2021 - JavaScript Entwicklungsumgebung

TypeScript ist seit vielen Jahre eine echte Alternative zu JavaScript und wird vor allem in Frameworks wie React, Angular und Vue verwendet. Das JavaScript für Backend-Entwickler punktet mit optionaler statischer Typisierung und einem schnellen intelligenten Compiler. Zusätzlich ist mit Interfaces und Modifiern echte objekt­orientierte Entwicklung möglich. Das alles prädestiniert es für den Einsatz in großen Projekten. Abgerundet wird es durch die Bereitstellung von Features aus zukünftigen JavaScript-Versionen, die größtenteils zu ECMAScript 3/5 transpiliert werden können und damit voll abwärtskompatibel zum JavaScript-Sprachstandard sind.

Bei dem verwendeten Repository handelt es sich um eine "Test-/Entwicklungsumgebung für JavaScript und TypeScript". Sie basiert auf Gulp, TypeScript/JS, ES6+ und Sass. Folgend die verwendeten NODE und NPM Versionen unter MacOS X 10.15.7 und Windows 10:

## MAC X 10.15.7:
NODE 14.18.1
NPM 6.14.15

## WINDOWS 10:
NODE 12.22.7
NPM 6.14.15

## Befehle
`npm install` ist der Befehl, der alle Packages installiert und alle Abhänigkeiten auflöst.

`npm run dev` ist der Befehl, der für das Starten der Umgebung erforderlich ist, alles auf einmal baut und auf Änderungen wartet. Hierbei wird ein Liveserver inkl. Browser-Refresh gestartet.

`npm run build` ist der Build-Befehl, hierbei wird alles gebaut und im `dist/` Verzeichnis hinterlegt. Es wird nicht auf Änderungen an Dateien gewartet.

Mit `npm run build:prod` kann ein Produktion Build erzeugt werden das keine Sourcemaps besitzt.

## Typescript

Zur Verwendung von Typescript muss eine in der Gulpfile die Variable `useTypeScript` auf `true` gesetzt werden. Anschließend werden die `.ts` Files in der `src/script` Directory genutzt und nicht mehr die `.js` Files. Es können jedoch beide Arten von Files in der Directory liegen.
