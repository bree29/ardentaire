# A.R. Dentaire bashscripts
## Introduction
Ce bashcript a été codé dans le but d'automatiser les tâches réalisées dans la cadre des missions de l'Association pour le Ronéo Dentaire (ARD).

Il comporte le script ardentaire, et sa dépendance mergeallpdf.
Vous devez installer, d'autre part, les paquets pdftk et wkhtmltopdf qui sont nécessaires à leur exécution.

Il assemble in fine les différents PDFs de chaque dossier présents dans le répertoire courant dans un seul fichier PDF "PolyToPrint.pdf" ; en respectant le "recto-verso" ; avec une output pour chacune des variables de StampList.

Il comporte trois phases :
- 1. la mise en place de la page de garde,
- 2. l'assemblage de chaque poly,
- 3. la personnalisation de chaque poly, en fonction de la demande.

---------------------------------------------------------------

Celui-ci nécessite d'être utilisé dans les bonnes conditions :
- Le répertoire courant ne doit pas contenir d'autres fichiers que PolyToPrint.pdf, qui est automatiquement supprimé au lancement du script ; et PDG.pdf qui sera la page de garde.
- Les répertoires comportant les PDF doivent avoir le titre de l'assemblage
- Chaque répertoire doivent contenir un fichier stamplist, contenant les différents noms des personnes pour qui sont imprimés les polys

---------------------------------------------------------------------

Cette procédure d'installation permet d'acquérir les versions les plus à jours de l'A.R. Dentaire. Ces versions sont normalement testées avant upload, mais ne sont pas, en soi, des versions définitives.

## Dernières updates (+/- expérimentales)
### Installation
    wget https://raw.githubusercontent.com/bree29/ardentaire/master/install-ard
    chmod +x install-ard && ./install-ard
### Update
    wget https://raw.githubusercontent.com/bree29/ardentaire/master/update-ard
    chmod +x update-ard && ./update-ard

## Dernière release stable
### Installation
    wget https://github.com/bree29/ardentaire/archive/V0.1a.tar.gz
    tar -zxvf V0.1a.tar.gz ./ardentaire-0.1a/install-ard
### Update
    wget https://github.com/bree29/ardentaire/archive/V0.1a.tar.gz
    tar -zxvf V0.1a.tar.gz ./ardentaire-0.1a/update-ard
