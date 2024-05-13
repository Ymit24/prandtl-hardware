# ❄️🎛️ Too Hot To Prandtl Hardware

## About this repo
This repo contains all the hardware I designed for my undergraduate senior design project "Too Hot To Prandtl".

<!-- TABLE OF CONTENTS -->
<div>
  <h4>Table of Contents</h4>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</div>


## About the Project
My senior design project, "Too hot to prandtl", is a thermal management solution designed for heterogeniously packaged chips.
It is a fluid based cooler which leverages phase change to increase heat transfer.
Myself, along with four Mechnical Engineering students designed, simulated, fabricated, and tested this system.
As the teams sole Electrical Engineer, I wrote all the software and designed, ordered, assembled, and brought-up the custom embedded system's printed circuit board (PCB).
The software for this project is hosted in a seperate repository found [here](https://github.com/Ymit24/too-hot-to-prandtl-control-system/tree/main).

![image](https://github.com/Ymit24/prandtl-hardware/assets/20305502/ab6c30c3-db80-439d-9537-be21344f3feb)


## Project Structure
This system is designed in KiCad. Any non-default symbols/footprints/models are located in the `lib/` directory and included in the custom symbols and footprints libraries.
Production files which were used for the prototype system are in the `production/` directory.

### Built With
- [KiCad](https://www.kicad.org), awesome free PCB designing tool!

## Roadmap
There are several design flaws in the first version of this system, all of which were able to be fixed in the lab so that the board was still operable.
Below are a few issues which I would address in a revision B, ordered from most severe to least.

- ESD protection diode is connected incorrectly. I misread the data sheet and connected the channels incorrectly.
- Serial wire debug header is both the wrong size/type and the footprint had a different pin labelling scheme than intended.
- Fan peripheral header needs power and ground connection.
- Use a single 8-bit/channel logic level shifter rather than eight individual 1-bit/channel shifters.
- Choose dimmer LEDs, the ones choosen are very bright.
- Fix typo in silkscreen for board name "Too Hot Too Prandtl" -> "Too Hot To Prandtl".

## License
This project uses the GNU General Purpose License (GPL). Basically, do whatever you want but you must open source any derivative work!

## Contact
My name is Christian Smith and you can contact me through my linked in [here](https://www.linkedin.com/in/christian-ryan-smith/).
As this was a senior design project which has now concluded, further work and support of this project will not continue.
