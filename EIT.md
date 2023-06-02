# Hilfreich für EIT Studenten

## anderes

### Docking Stations in der Fachschaft

* Webseite: <https://i-tec.pro/de/produkt/u3hdmidvidock-3/>
* Treiber:  <https://i-tec.cz/wp-content/uploads/man_dri/DisplayLink_Ubuntu.zip>


## Fächer

### Info 1&2

* `sudo apt install gcc`

### Gleichstromtechnik

* LTSpice: leider nur mit Wine.
* KiCad: (<https://www.kicad.org/download/ubuntu/>)
  * `sudo add-apt-repository --yes ppa:kicad/kicad-7.0-releases`
  * `sudo apt update`
  * `sudo apt install --install-recommends kicad`

### Digitaltechnik/EDS

* Vivado: (<https://www.xilinx.com/support/download.html>)

### ModSim

* Python: `sudo apt install python3 python3-numpy python3-scipy python3-matplotlib`
* OpenModelica: (<https://openmodelica.org/download/download-linux>)
  * requirements: `wget`, `pip`, `tee`
  1) `echo "deb-src https://build.openmodelica.org/apt stable" | sudo tee -a /etc/apt/sources.list.d/openmodelica.list`
  2) `wget -q http://build.openmodelica.org/apt/openmodelica.asc -O- | sudo apt-key add -`
  3) `sudo apt update`
  4) `sudo apt install openmodelica`
  5) `python -m pip install -U https://github.com/OpenModelica/OMPython/archive/master.zip`

### Elektronik Labor

* Cadance: `ssh -Y n4-caee-01@EIT-CAEE-S02.Hs-Karlsruhe.de`

### Regelungstechnik

* Matlab/Simulink: <https://de.mathworks.com/support/requirements/matlab-linux.html>

### Hochfrequenztechnik

* Keysight ADS: [Download](https://www.keysight.com/de/de/lib/software-detail/computer-software/pathwave-advanced-design-system-ads-software-2212036/ads-2023-linux.html)
