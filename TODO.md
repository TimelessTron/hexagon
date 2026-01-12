# 📦 PHP Testing- & Analyse-Toolbox

## 🧪 Unit- & Feature-Test-Frameworks

| Framework        | Beschreibung                                                                                                   | Doku                           |
| ---------------- |----------------------------------------------------------------------------------------------------------------|--------------------------------|
| **PHPUnit**      | 🏆 De-facto-Standard für Unit-Tests. Mit Mocks, Data-Providern, Assertions etc.                                | https://phpunit.de/            |
| **Pest**         | 🧼 Moderner, lesbarer Wrapper für PHPUnit. Ideal für elegante Tests.                                           | https://pestphp.com/           |
| **Codeception**  | 🔦 Kombiniert Unit-, Functional- & Acceptance-Tests (z. B. REST, Gherkin, Browser).                            | https://codeception.com/       |
| **Nette Tester** | ⚡ Leichtgewichtig & schnell. Kommt aus dem Nette-Ökosystem.                                                    | https://github.com/nette/tester |
| **Atoum**        | 🧪 Französisches Framework mit DSL-Ansatz. Weniger verbreitet, aber spannend.                                  | https://atoum.org/             |

## 🧠 Behavior Driven Development (BDD)

| Framework   | Beschreibung                                                                                                  | Doku                |
| ----------- |---------------------------------------------------------------------------------------------------------------|---------------------|
| **PHPSpec** | 🧠 BDD-Tool mit Fokus auf objektbasiertes Design (Verhalten statt Implementierung).                          | http://www.phpspec.net/ |
| **Behat**   | 💬 Feature-Tests in natürlicher Sprache (Gherkin-Syntax: Given/When/Then).                                     | https://behat.org/  |

## 🧠 Statische Analyse

| Tool        | Beschreibung                                                     | Doku                         |
|-------------|------------------------------------------------------------------|------------------------------|
| **PHPStan** | 🚨 Erkennt viele Fehler zur Analysezeit. Unterstützt Level 0–9.  | https://phpstan.org/         |
| **Psalm**   | 🧙 Sehr strikt. Bietet Taint Analysis, Type Coverage, Generics.  | https://psalm.dev/           |
| **Phan**    | 🦕 Früheres Static-Tool, heute weniger verbreitet.               | https://github.com/phan/phan |

## 📊 Testabdeckung & Mutation Testing

| Tool                      | Beschreibung                                                                | Doku                                               |
|---------------------------|-----------------------------------------------------------------------------|----------------------------------------------------|
| **PHPUnit Code Coverage** | 📊 Integriert in PHPUnit. Nutzt Xdebug/PCOV zur Coverage-Messung.           | https://docs.phpunit.de/en/12.2/code-coverage.html |
| **Infection**             | 🧬 Mutation Testing: injiziert Fehler in deinen Code, prüft Teststabilität. | https://infection.github.io/                       |

## 🚨 Sicherheitsanalyse

| Tool                            | Beschreibung                                                                    | Doku                                          |
|---------------------------------|---------------------------------------------------------------------------------|-----------------------------------------------|
| **Psalm (Taint plugin)**        | 🛡️ Analysiert potenziell unsichere Datenflüsse (User-Input → DB etc.).         | https://psalm.dev/docs/security_analysis/     |
| **Roave/BetterReflection**      | 🔬 Reflection-Analyse, z. B. zur Laufzeitanalyse oder Code-Introspektion.       | https://github.com/Roave/BetterReflection     |
| **Security Advisories Checker** | 🔒 CLI-Tool zur Prüfung von Composer-Dependencies auf Sicherheitslücken.        | https://github.com/Roave/SecurityAdvisories   |

## 🏗️ Architektur / Struktur / Komplexität

| Tool                        | Beschreibung                                                                        | Doku                                  |
|-----------------------------|-------------------------------------------------------------------------------------|---------------------------------------|
| **Deptrac**                 | 🕸️ Erzwingt Schichtenarchitektur (z. B. Domain → kein Zugriff auf Infrastructure). | https://github.com/deptrac/deptrac    |
| **PHP Architecture Tester** | 📏 Erzwingt Architekturregeln für Klassen, Layer & Namensräume.                     | https://www.phpat.dev/                |
| **PHPMetrics**              | 📈 Metriken (z. B. Komplexität, Größe, Abhängigkeiten) + schöne HTML-Reports.       | https://phpmetrics.org/               |
| **PHPDepend**               | 📉 Analyse von Abstractness, Instabilität, Afferent/Efferent Coupling usw.          | https://pdepend.org/                  |
| **PHPLOC**                  | 🧮 Zählt Zeilen, Klassen, Methoden, Coverage etc. Ideal für CI-Reports.             | https://phpqa.io/projects/phploc.html |

## 🎨 Code Style & Linter

| Tool                         | Beschreibung                                                 | Doku                                                         |
|------------------------------|--------------------------------------------------------------|--------------------------------------------------------------|
| **PHP-CS-Fixer**             | 🧽 Auto-Fixer nach PSR-Standards. Sehr anpassbar.            | https://github.com/PHP-CS-Fixer/PHP-CS-Fixer                 |
| **PHP_CodeSniffer (phpcs)**  | 🔎 Prüft Style-Konventionen wie PSR-12, Zend, Symfony.       | https://github.com/squizlabs/PHP_CodeSniffer                 |
| **EasyCodingStandard (ECS)** | 🧠 Kombiniert Fixer + Sniffer + mehr. Top Tool von Symplify. | https://github.com/easy-coding-standard/easy-coding-standard |

## 🧰 Weitere Tools & Erweiterungen

| Tool                   | Beschreibung                                                       | Doku                                           |
|------------------------|--------------------------------------------------------------------|------------------------------------------------|
| **Mockery**            | 🎭 Flexibles Mocking-Tool für PHPUnit oder Pest.                   | https://github.com/mockery/mockery             |
| **Prophecy**           | 🔮 Default in PHPSpec. In PHPUnit deprecated, aber noch verfügbar. | https://github.com/phpspec/prophecy            |
| **Rector**             | 🧙 Automatisierte Refactorings & PHP-Version-Upgrades.             | https://github.com/rectorphp/rector            |
| **Composer Normalize** | 🔧 Vereinheitlicht `composer.json`. Ideal für CI.                  | https://github.com/ergebnis/composer-normalize |
| **PHPStan Deployer**   | 🛠️ Für strukturierte, modularisierte Deployments mit Regeln.      | https://github.com/deployphp/deployer          |

## 📚 Tools zur Generierung von Dokumentation aus PHP-Code

| Tool               | Beschreibung                                                                                          | Doku                                         |
|--------------------|-------------------------------------------------------------------------------------------------------|----------------------------------------------|
| **phpDocumentor**  | 🏛️ Der Klassiker – generiert HTML/PDF-Doku aus PHPDoc-Kommentaren. Unterstützt viele Tags & Layouts. | https://phpdoc.org/                          |
| **Doctum**         | ⚡ Schneller Fork von Sami (ehem. Symfony). Leichtgewichtig und CI-freundlich.                         | https://github.com/code-lts/doctum           |
| **Doxygen**        | 🧪 Nicht PHP-spezifisch, aber unterstützt es. Vielseitig, aber etwas veraltet in PHP-Projekten.       | https://www.doxygen.nl/manual/docblocks.html |
| **ApiGen**         | 📘 PHPDoc-basierte Generator-Alternative. Nicht mehr sehr aktiv, aber noch brauchbar.                 | https://github.com/ApiGen/ApiGen             |
| **Swagger-PHP**    | 🧬 Erstellt OpenAPI-Spezifikationen (JSON/YAML) für REST-APIs anhand von PHP-Attributen/PHPDocs.      | https://zircote.github.io/swagger-php/       |
