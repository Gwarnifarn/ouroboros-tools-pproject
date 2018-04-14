<table style="text-align: left; font-size: 18px">
    <tr>
        <td>Twitter</td>
        <td>@simon\_kallfass</td>
    </tr>
    <tr>
        <td>GitHub</td>
        <td>skallfass</td>
    </tr>
    <tr>
        <td>GitLab</td>
        <td>skallfass</td>
    </tr>
    <tr>
        <td>LinkedIn</td>
        <td>Simon Kallfaß</td>
    </tr>
    <tr>
        <td>Homepage</td>
        <td>[www.ouroboros.info](https://www.ouroboros.info)</td>
    </tr>
</table>

<img src="https://pproject.ouroboros.info/_images/pproject.svg" alt="pproject logo" width="30%" height="30%" z-index=-5 style="background-color: #434344;">

[www.pproject.ouroboros.info](https://www.pproject.ouroboros.info)

---

## Warum pproject?
* Vereinfachung von
    * Entwicklung in Conda-Environments
    * Ausrollen als Conda-Packages
* VCS
    * Repository anlegen
    * git-tags
* feste Projektstruktur
    * gleicher Aufbau
    * vorhersehbarer Inhalt
* als Playground für Packages & Technologien

---

## Features
* Shell-tool (bash und zsh)
* Projekterstellung (lokal / remote)
* Conda-Environments (erstellen und updaten)
* Tests (pytest)
* Conda-Packages
* Rollout (als Conda-Package in eigenem Conda-Env)
* Sphinx

---

## Resultierende Projektstruktur
```
├── conda-build
│       ├── meta.yaml
│       └── hash.md5
├── company
│       ├── init__.py
│       └── namespace
│           ├── init__.py
│           └── project
│               ├── your_code.py
│               └── __init__.py
├── .git
├── README.md
├── setup.py
└── tests
```

---

[![Example](https://asciinema.org/a/172085.png)](https://asciinema.org/a/172085)

---

### Development-Circle
<img src="https://pproject.ouroboros.info/_images/development_circle.svg" alt="Development-Circle" width="50%" height="50%">

---

## Erstellen und Entwickeln
Erstellen:
```bash
pproject create --remote tools example -p 3.6
```
Update des Conda-Envs:
```bash
pproject update
```
Testen:
```bash
pproject test
```

---
## Status und Build
Überblick:
```bash
pproject info {project, general}
```
Neuer Versionstag:
```bash
pproject version -m "MESSAGE" {major, minor, patch}
```
Conda-Package erstellen:
```bash
pproject build [--publish]
```

---
## Ausrollen und Dokumentation
Ausrollen auf Host:
```bash
pproject release -d USER@HOST -e ENVIRONMENT_NAME
```
Erstellen der Sphinx-Dokumentation:
```bash
pproject sphinx
```

---

## Ausblick
* eventuell Bitbucket-support
* fish-support
* flexiblere Namespaces
* Plugin-System?
* Neuer Befehl: "containerize/dockerize/..."
* CI-Skeletons?

---

## Contributors welcome!
<table style="text-align: left; font-size: 18px">
    <tr>
        <td>Homepage</td>
        <td>https://www.pproject.ouroboros.info</td>
    </tr>
    <tr>
        <td>GitHub</td>
        <td>skallfass/ouroboros-tools-pproject</td>
    </tr>
    <tr>
        <td>GitLab</td>
        <td>ouroboros-tools/pproject</td>
    </tr>
</table>