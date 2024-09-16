
# TPMS Viewer

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

## Description

An interactive online viewer to explore and visualize **Triply Periodic Minimal Surfaces (TPMS)**. This web app allows users to view various types of TPMS surfaces, adjust their thickness, and export the results to an OBJ file. The app uses the **marching cubes algorithm** to generate TPMS surfaces, allowing real-time rendering and surface customization. The generated 3D models can be exported as an OBJ file. The app is built using [Three.js](https://threejs.org/), and it requires a web server to host the HTML and JavaScript files.

### Demo

Check out the live demo here: [https://cise.ufl.edu/~p.gupta/tpms-viewer/](https://cise.ufl.edu/~p.gupta/tpms-viewer/)

### Supported TPMS Types

| **TPMS Type**  | **Equation** |
|----------------|--------------|
| Schwarz P      | cos(x) + cos(y) + cos(z) = 0 |
| Gyroid         | sin(x)cos(y) + sin(y)cos(z) + sin(z)cos(x) = 0 |
| Nevious        | 3(cos(x) + cos(y) + cos(z)) + 4(cos(x)cos(y)cos(z)) = 0 |
| Lidinoid       | 0.5[sin(2x)cos(y)sin(z) + sin(2y)cos(z)sin(x) + sin(2z)cos(x)sin(y)] - 0.5[cos(2x)cos(2y) + cos(2y)cos(2z) + cos(2z)cos(2x)] + 0.15 = 0 |
| PW Hybrid      | 2(cos(x)cos(y) + cos(y)cos(z) + cos(z)cos(x)) - 4(cos(x)cos(y)cos(z)) + 0.24 = 0 |
| Diamond        | sin(x)sin(y)sin(z) + sin(x)cos(y)cos(z) + cos(x)sin(y)cos(z) + cos(x)cos(y)sin(z) = 0 |
| Split P        | 1.1[sin(2x)sin(z)cos(y) + sin(2y)sin(x)cos(z) + sin(2z)sin(y)cos(x)] - 0.2[cos(2x)cos(2y) + cos(2y)cos(2z) + cos(2z)cos(2x)] - 0.4(cos(2x) + cos(2y) + cos(2z)) = 0 |


## Table of Contents

-   [Installation](#installation)
-   [How It Works](#how-it-works)
-   [License](#license)
-   [Contact](#contact)

## Installation

1.  Clone or download this repository.
2.  Host the app on any web server.
3.  Open the app in a modern web browser.

## How It Works

The web app uses the **marching cubes algorithm** to create 3D meshes representing TPMS surfaces. This algorithm takes a scalar field that describes the TPMS geometry and generates a surface by constructing polygons around threshold values. Users can adjust the thickness of the surface to see the TPMS in different forms. The final surface can then be exported as an OBJ file for further use.

## License

This project is licensed under the [MIT License](LICENSE).

## Contact

If you have any questions or suggestions, feel free to contact me at [p.gupta@ufl.edu](mailto:p.gupta@ufl.edu).