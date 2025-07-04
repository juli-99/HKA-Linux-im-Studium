# Hilfreich für IWI Studenten

## Generelles

### [Mattermost](https://mattermost.com/)
Direkt im Browser oder
[installations Anleitung](https://docs.mattermost.com/collaborate/install-desktop-app.html)

## Fächer
<details>
<summary>
  
  ### Semester 1
  
</summary>

#### Mathe Labor

[Python](https://www.python.org/) mit Libraries ([numpy](https://numpy.org/), [sympy](https://www.sympy.org), mpmath und [Matplotlib](https://matplotlib.org/)) und [Jupyter Notebooks](https://jupyter.org/).  
Es gibt drei Möglichkeiten diese zu installieren:

1. Über [Anaconda](https://www.anaconda.com/) wie in der Labor Anleitung beschrieben.
2. Über den Packetmanager der Distribution.
   * `sudo apt install python3`
   * `sudo apt install python3-numpy python3-sympy python3-mpmath python3-matplotlib`
   * `sudo apt install jupyter`
3. Über [PIP](https://pypi.org/).
   * Setzt Python und PIP voraus. Ein [Guide](https://packaging.python.org/en/latest/tutorials/installing-packages/) welcher die Instalation und Benutzung von PIP erklärt.
   * `pip install numpy sympy mpmath matplotlib`
   * `pip install jupyterlab`

#### Programieren

* Java: `sudo apt install openjdk-17-jdk`
* Hexviewer:
  * `hexdump` [man](https://man7.org/linux/man-pages/man1/hexdump.1.html)
  * [GHex](https://gitlab.gnome.org/GNOME/ghex)`sudo apt install ghex`
</details>

<details>
<summary>
  
  ### Semester 2
  
</summary>

#### Algorithmen und Datenstrukturen Labor

* [Java](https://openjdk.org): `sudo apt install openjdk-17-jdk`
</details>

<details>
<summary>
  
  ### Semester 3
  
</summary>

#### Kommunikationsnetze 1 Vorlesung

* telnet
* [Wireshark](https://www.wireshark.org/): `sudo apt install wireshark`

#### Kommunikationsnetze 1 Labor

Benutze die gegbene VM alles andere ist deutlich komplizierter.

* [VirtualBox](https://www.virtualbox.org/): `sudo apt install virtualbox`

#### Betriebssysteme Labor

* [git](https://git-scm.com/): `sudo apt install git`
* [gcc](https://gcc.gnu.org/): `sudo apt install gcc`
* make: `sudo apt install make`
* [cmake](https://cmake.org/) `sudo apt install cmake`

#### Datenbanken Labor

* [DBeaver](https://dbeaver.io/)
* optional locale Datenbank:
  * [PostgreSQL](https://www.postgresql.org)
  * [MariaDB](https://mariadb.org)

### Deklarative Programmierung

* [Eclipse JEE](https://www.eclipse.org/downloads/packages/release/2023-09/r/eclipse-ide-enterprise-java-and-web-developers)

alternativ

* node module [xslt3](https://www.npmjs.com/package/xslt3)
* optional VS Code mit [XSLT/XPath extention](https://marketplace.visualstudio.com/items?itemName=deltaxml.xslt-xpath)

### Maschinelles Lernen

* [Python](https://www.python.org/) und [Jupyter Notebooks](https://jupyter.org/), siehe [Mathe Labor](#mathe-labor)
* zusätzlich [Pandas](https://pandas.pydata.org/) und [scikit-learn](https://scikit-learn.org/stable/) installieren

</details>

<details>
<summary>
  
  ### Semester 4
  
</summary>

#### Praxisvorbereitung

Siehe [LaTeX](Generell.md#latex) in [Generell](Generell.md).


</details>

<details>
<summary>
  
  ### Semester 5
  
</summary>

#### Computergrafik

* [gcc](https://gcc.gnu.org/): `sudo apt install gcc`
* make: `sudo apt install make`
* [cmake](https://cmake.org/) `sudo apt install cmake`
* [gtest](https://github.com/google/googletest) Bibiliothek.

#### Verteilte Systeme 2

* [git](https://git-scm.com/): `sudo apt install git`

##### Mit Docker

* [VS Code](https://code.visualstudio.com/)
  * [Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)
* [Docker Desktop](https://docs.docker.com/desktop/install/linux-install/)

##### Ohne Docker

* [Redis](https://redis.io/docs/install/install-redis/install-redis-on-linux/)
* Python
  * [RPyC](https://rpyc.readthedocs.io/en/latest/) `pip install rpyc`
  * [Redis](https://redis.io/docs/connect/clients/python/)
  * ([Pipenv](https://pipenv.pypa.io/en/latest/))

#### Softwareengeneering

* [Together](https://www.microfocus.com/de-de/products/together/overview) Per vorgegebene Anleitung.
  * ging direkt mit `OpenJDK 17`
  * `Together.ini` musste angepasst werden.
    * `-XX:MaxPermSize=256m` entfernt
    * `equinox` Plugin Version musste angepasst werden

#### ERP-Labor

1) `GUI770Installation_8-80004696.zip` von ILIAS herunterladen und entpacken.
2) Mit hilfe von `./PlatinGUI-Linux-Installation` installieren.
3) SAP-GUI starten mit `SAProuter-String` aus `SAP-Verbindungsdaten-Linux-macOS.txt`:
 ```bash
~/SAPClients/SAPGUI/bin/guistart <SAProuter-String>
```

ABAB:
Angeblich nicht für Linux ferfügbar funktioniert aber Problemlos.
Einfach den Tutorials folgen.
</details>

<details>
<summary>
  
  ### Semester 6
  
</summary>

### Autonome Systeme
Programmiersprache: [Go](https://go.dev/)  
* Über den [Packetmanager](https://repology.org/project/go/versions) (meist als golang)
* [Manuell](https://go.dev/doc/install)

Optional [Go VSCode extention](https://marketplace.visualstudio.com/items?itemName=golang.Go)

### Embedded Software
Programmiersprache: C/C++
* [gcc](https://gcc.gnu.org/)
* [Google Benchmark](https://github.com/google/benchmark)
* [hyperfine](https://github.com/sharkdp/hyperfine) Terminal Laufzeitmessung
* `perf` profiler
  * optionale GUI: [Hotspot](https://github.com/KDAB/hotspot)

</details>

<details>
<summary>
  
  ### Wahlfächer
  
</summary>

#### Parallele Systeme

* [CUDA Toolkit](https://developer.nvidia.com/cuda-downloads?target_os=Linux)

#### Ethical Hacking

* [Kali Linux](https://www.kali.org/get-kali/#kali-platforms)
* [VirtualBox](https://www.virtualbox.org/): `sudo apt install virtualbox`

</details>
