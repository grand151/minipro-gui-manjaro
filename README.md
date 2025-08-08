![minipro.jpg](res%2FAppIcon.ico)
# MINIPRO-GUI
### *GUI wrapper for the [minipro CLI tool](https://gitlab.com/DavidGriffith/minipro) - a free and open TL866 series programmer*

[![Unit Tests](https://github.com/twelve-chairs/minipro-gui/actions/workflows/tests.yaml/badge.svg)](https://github.com/twelve-chairs/minipro-gui/actions/workflows/tests.yaml)
[![Build Ubuntu](https://github.com/twelve-chairs/minipro-gui/actions/workflows/ubuntu.yaml/badge.svg)](https://github.com/twelve-chairs/minipro-gui/actions/workflows/ubuntu.yaml)
[![Build MacOS](https://github.com/twelve-chairs/minipro-gui/actions/workflows/macos.yaml/badge.svg)](https://github.com/twelve-chairs/minipro-gui/actions/workflows/macos.yaml)
[![CodeQL](https://github.com/twelve-chairs/minipro-gui/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/twelve-chairs/minipro-gui/actions/workflows/github-code-scanning/codeql) 
[![Sonar Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=twelve-chairs_minipro-gui&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=twelve-chairs_minipro-gui)

![screenshot.png](res%2Fscreenshot.png)
## Installation
Coming soon as pre-compiled binary releases. For now, please build from source.
## Dependencies
#### MacOS

```
brew install cmake ninja qt6 minipro
```

#### Ubuntu / Debian
Install minipro CLI (required): https://gitlab.com/DavidGriffith/minipro#install-build-dependencies

```
sudo apt-get install build-essential ninja-build cmake libgl1-mesa-dev qt6-base-dev -y
```

  (*If your OS uses Wayland (e.g. Raspberry PI 5), please also install `qt6-wayland` via apt-get*)

#### Fedora
Install minipro CLI (required): https://gitlab.com/DavidGriffith/minipro#install-build-dependencies

```
sudo dnf groupinstall "C Development Tools and Libraries"
sudo dnf install ninja-build cmake mesa-libGL-devel qt6-qtbase-devel -y
```

#### openSUSE
Install minipro CLI (required): https://gitlab.com/DavidGriffith/minipro#install-build-dependencies
```
sudo zypper install --type pattern devel_basis
sudo zypper install cmake Mesa-libGL-devel qt6-base-devel -y
```

#### Manjaro
Install minipro CLI (required): https://gitlab.com/DavidGriffith/minipro#install-build-dependencies

```
sudo pacman -Syu base-devel ninja cmake qt6-base mesa
```

## Build and run
```
git clone https://github.com/twelve-chairs/minipro-gui.git
cd minipro-gui
cmake -DCMAKE_BUILD_TYPE=MinSizeRel -DCMAKE_MAKE_PROGRAM=ninja -G Ninja -S . -B "./cmake-build-minsizerel"
cmake --build ./cmake-build-minsizerel --target minipro-gui -- -j 2
./cmake-build-minsizerel/minipro-gui
```

---

![minipro.jpg](res%2FAppIcon.ico)
# MINIPRO-GUI
### *Graficzna nakładka dla narzędzia CLI [minipro](https://gitlab.com/DavidGriffith/minipro) - darmowego i otwartego programatora serii TL866*

[![Testy jednostkowe](https://github.com/twelve-chairs/minipro-gui/actions/workflows/tests.yaml/badge.svg)](https://github.com/twelve-chairs/minipro-gui/actions/workflows/tests.yaml)
[![Kompilacja Ubuntu](https://github.com/twelve-chairs/minipro-gui/actions/workflows/ubuntu.yaml/badge.svg)](https://github.com/twelve-chairs/minipro-gui/actions/workflows/ubuntu.yaml)
[![Kompilacja MacOS](https://github.com/twelve-chairs/minipro-gui/actions/workflows/macos.yaml/badge.svg)](https://github.com/twelve-chairs/minipro-gui/actions/workflows/macos.yaml)
[![CodeQL](https://github.com/twelve-chairs/minipro-gui/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/twelve-chairs/minipro-gui/actions/workflows/github-code-scanning/codeql) 
[![Status bramki jakości Sonar](https://sonarcloud.io/api/project_badges/measure?project=twelve-chairs_minipro-gui&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=twelve-chairs_minipro-gui)

![screenshot.png](res%2Fscreenshot.png)
## Instalacja
Wkrótce dostępne będą gotowe wydania binarne. Na razie prosimy o kompilację ze źródła.
## Zależności
#### MacOS

```
brew install cmake ninja qt6 minipro
```

#### Ubuntu / Debian
Zainstaluj narzędzie CLI minipro (wymagane): https://gitlab.com/DavidGriffith/minipro#install-build-dependencies

```
sudo apt-get install build-essential ninja-build cmake libgl1-mesa-dev qt6-base-dev -y
```

  (*Jeśli Twój system operacyjny używa Wayland (np. Raspberry PI 5), zainstaluj również `qt6-wayland` za pomocą apt-get*)

#### Fedora
Zainstaluj narzędzie CLI minipro (wymagane): https://gitlab.com/DavidGriffith/minipro#install-build-dependencies

```
sudo dnf groupinstall "C Development Tools and Libraries"
sudo dnf install ninja-build cmake mesa-libGL-devel qt6-qtbase-devel -y
```

#### openSUSE
Zainstaluj narzędzie CLI minipro (wymagane): https://gitlab.com/DavidGriffith/minipro#install-build-dependencies
```
sudo zypper install --type pattern devel_basis
sudo zypper install cmake Mesa-libGL-devel qt6-base-devel -y
```

#### Manjaro
Zainstaluj narzędzie CLI minipro (wymagane): https://gitlab.com/DavidGriffith/minipro#install-build-dependencies

```
sudo pacman -Syu base-devel ninja cmake qt6-base mesa
```

## Budowanie i uruchamianie
```
git clone https://github.com/twelve-chairs/minipro-gui.git
cd minipro-gui
cmake -DCMAKE_BUILD_TYPE=MinSizeRel -DCMAKE_MAKE_PROGRAM=ninja -G Ninja -S . -B "./cmake-build-minsizerel"
cmake --build ./cmake-build-minsizerel --target minipro-gui -- -j 2
./cmake-build-minsizerel/minipro-gui
