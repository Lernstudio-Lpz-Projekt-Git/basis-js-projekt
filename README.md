# Basis Javascript Projekt- und Entwicklungsumgebung

Bei diesem Repository handelt es sich um eine "Test-/Entwicklungsumgebung" die auf Gulp, TypeScript/JS, ES6+ und Sass basiert.

# IDE 11/2021 - JavaScript Entwicklungsumgebung

TypeScript ist seit vielen Jahre eine echte Alternative zu JavaScript und wird vor allem in Frameworks wie React, Angular und Vue verwendet. Das JavaScript für Backend-Entwickler punktet mit optionaler statischer Typisierung und einem schnellen intelligenten Compiler. Zusätzlich ist mit Interfaces und Modifiern echte objekt­orientierte Entwicklung möglich. Das alles prädestiniert es für den Einsatz in großen Projekten. Abgerundet wird es durch die Bereitstellung von Features aus zukünftigen JavaScript-Versionen, die größtenteils zu ECMAScript 3/5 transpiliert werden können und damit voll abwärtskompatibel zum JavaScript-Sprachstandard sind.

Bei dem verwendeten Repository handelt es sich um eine "Test-/Entwicklungsumgebung für JavaScript und TypeScript". Sie basiert auf Gulp, TypeScript/JS, ES6+ und Sass. Folgend die verwendeten NODE und NPM Versionen unter MacOS X 10.15.7 und Windows 10:

## MAC X 10.15.7:
NODE 14.18.1\
NPM 6.14.15

## WINDOWS 10:
NODE 12.22.7\
NPM 6.14.15

## Installierte Node Versionen prüfen
Nach der Installtion sollten wir die Versionen von node, npm, and npx prüfen! Im ergebnis sollten folgende Versionen installiert sein:
`node -v //v12.22.7`\
`npm -v //6.14.15` NPM - verwaltet Pakete, kann aber keine pakete ausführen, Pakete auszuführen. \
`npx -v //6.14.15` NPX - ein Tool zum Ausführen von Node-Paketen.

## Gulp installieren und neues Projekt erstellen
Wenn Sie gulp bereits global installiert haben, führen Sie `npm rm --global gulp`  aus um ihre Version zu deinstallieren.\
Danach installieren Sie das Kommandozeilenprogramm gulp: `npm --global gulp-cli`
Erzeugen ein Projektverzeichnis: `npx mkdirp my-project` oder wechseln Sie ihr Projektverzeichnis `cd my-project`
Erstellen Sie eine package.json-Datei in Ihrem Projektverzeichnis: `npm init`
Installieren Sie das gulp-Paket ihrer dev-Abhängigkeiten aus der package.json: `npm install --save-dev gulp`
Überprüfen Sie Ihre Gulp-Versionen: `gulp --version`

## Befehle
`npm install` ist der Befehl, der alle Packages installiert und alle Abhänigkeiten auflöst.

`npm run dev` ist der Befehl, der für das Starten der Umgebung erforderlich ist, alles auf einmal baut und auf Änderungen wartet. Hierbei wird ein Liveserver inkl. Browser-Refresh gestartet.

`npm run build` ist der Build-Befehl, hierbei wird alles gebaut und im `dist/` Verzeichnis hinterlegt. Es wird nicht auf Änderungen an Dateien gewartet.

Mit `npm run build:prod` kann ein Produktion Build erzeugt werden das keine Sourcemaps besitzt.

## Typescript

Zur Verwendung von Typescript muss eine in der Gulpfile die Variable `useTypeScript` auf `true` gesetzt werden. Anschließend werden die `.ts` Files in der `src/script` Directory genutzt und nicht mehr die `.js` Files. Es können jedoch beide Arten von Files in der Directory liegen.
