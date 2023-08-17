# Hilfreich für EIT Studenten

## anderes

### Docking Stations in der Fachschaft

* [Webseite](https://i-tec.pro/de/produkt/u3hdmidvidock-3/)
* [Treiber](https://i-tec.cz/wp-content/uploads/man_dri/DisplayLink_Ubuntu.zip)

## Fächer

### Info 1&2
* C & C++ Compiler:
  * [GCC](https://gcc.gnu.org/): `sudo apt install gcc`
* optional IDE:
  *  [Visual Studio Code](https://code.visualstudio.com/): https://code.visualstudio.com/docs/setup/linux
  *  [Eclipse](https://www.eclipse.org/downloads/packages/): https://www.eclipse.org/downloads/packages/installer

### Gleichstromtechnik

* [LTSpice](https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html):
  * leider nur mit [Wine](https://www.winehq.org/).
  * end of support Januar 2023
* [KiCad](https://www.kicad.org/):
  * https://www.kicad.org/download/linux/

### Digitaltechnik/EDS

* [Vivado](https://www.xilinx.com/support/download.html)
* Logic-simulator:
  * [Logisim-evolution](https://github.com/logisim-evolution/logisim-evolution)
  * [Digital](https://github.com/hneemann/Digital)

### ModSim

* [Python](https://www.python.org/): `sudo apt install python3 python3-numpy python3-scipy python3-matplotlib`
* [OpenModelica](https://openmodelica.org/download/download-linux):
  * requirements: `wget`, `pip`, `tee`
  ```bash
  # 1. OpenModelica repository zu APT quellen hinzufügen
  echo "deb-src https://build.openmodelica.org/apt stable" | sudo tee -a /etc/apt/sources.list.d/openmodelica.list
  wget -q http://build.openmodelica.org/apt/openmodelica.asc -O- | sudo apt-key add -
  # 2. Paketquelle "aktivieren"
  sudo apt update
  # 3. OpenModelica installieren
  sudo apt install openmodelica
  # 4. OMPython installieren
  python -m pip install -U https://github.com/OpenModelica/OMPython/archive/master.zip
  ```

### Elektronik Labor

* Cadance: `ssh -Y n4-caee-01@EIT-CAEE-S02.Hs-Karlsruhe.de`

### Regelungstechnik

* [Matlab/Simulink](https://de.mathworks.com/support/requirements/matlab-linux.html)

### Hochfrequenztechnik

* [Keysight ADS](https://www.keysight.com/de/de/lib/software-detail/computer-software/pathwave-advanced-design-system-ads-software-2212036/ads-2023-linux.html)

### Digitale Signal Prozesoren

* [Matlab](https://de.mathworks.com/support/requirements/matlab-linux.html)
* alternativ [GNU Octave](https://www.octave.org/)
  * [signal](https://gnu-octave.github.io/packages/signal/) (dependency: [control](https://gnu-octave.github.io/packages/control/))
