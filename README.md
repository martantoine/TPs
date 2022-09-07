# Introduction
Bienvenue dans ce tout premier TP du cours MICRO-315

# Partie 1 - Environnement de développement (IDE)
Cliquer sur l'un des liens suivant selon votre configuration
- 👉[❖ Windows](https://github.com/epfl-mobots/MICRO-315-TPs-Student/wiki/Installation-de-l'IDE---%E2%9D%96-Windows)
- 👉[🍎 MacOS](https://github.com/epfl-mobots/MICRO-315-TPs-Student/wiki/Installation-de-l'IDE---%E2%9D%96-Windows)
- 👉[🐧 Linux](https://github.com/epfl-mobots/MICRO-315-TPs-Student/wiki/Installation-de-l'IDE---%E2%9D%96-Windows)

# Structure des outils de IDE
Les principaux outils utilisés sont:
- Visual Studio Code, ses extensions:
    - C/C++ de Microsoft
    - Cortex-Debug de marus25
    - Task Runner
- Git
- Git credential manager
- ARM Toolchain
- CortexDebug
- Make

Le dossier d'installation est structuré de la manière suivante:
```
Installation folder
 │
 ├── ...
 ├── EPuck2Tools
 │   ├── Utils
 │   │   ├── STM32F407.svd			    : Fichier indispensable au Debogueur pour lire les registres
 │   │   │                                 des périphériques du STM32F406
 │   │   ├── dfu-util.exe			    : Programmeur en mode DFU
 │   │   ├── e-puck2_main-processor.bin	: Programme démo de l'EPuck2
 │   │   └── zadig-2.3.exe
 │   └── gcc-arm-none-eabi-7-2017-q4-major
 │       ├── ...
 │       ├── bin
 │       │   │
 │       │   ├── ...
 │       │   ├── arm-none-eabi-gcc.exe	: Compilateur
 │       │   ├── ...
 │       │   ├── arm-none-eabi-gdb.exe	: Debogueur
 │       │   └── ...
 │       └── ...
 ├── VSCode_EPuck2
 │   ├── ...
 │   ├── data
 │   │   ├── extensions			        : Contiens les extensions
 │   │   └── user-data                  : Fichiers de configurations
 │   └── ...
 └── ...
```

### Workplace_EPuck2
Le dossier **Workplace_EPuck2** contient toutes les librairies utilisées pour les TPs et le mini-projet de ce cours.
La librairie standard C est contenue dans *gcc-arm-none-eabi-7-2017-q4-major*.
C'est aussi dans **Workplace_EPuck2** que seront stockés les TPs et le mini-projet.
Le dossier de travail **Workplace_EPuck2** est structuré de la manière suivante:
```
Workplace_EPuck2
 │
 ├── Lib
 │   ├── e-puck2_main-processor
 │   ├── example project
 │   └── ST
 ├── TP1
 ├── TP2
 └── ...
 ```

 ### Premier demarrage
VSCode_EPuck2 étant maintenant installé, il est temps de tester l'IDE avec un projet exemple pour s'habituer aux outils et vérifier leur bon fonctionnement 

<img src="pictures/Capture.PNG" alt="drawing" width="500"/>
### Présentation de l'outil
#### Hierarchie des outils
#### Interface de 