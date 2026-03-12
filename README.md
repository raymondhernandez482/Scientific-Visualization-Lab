# Scientific Visualization Lab

Experiments in scientific data visualization and simulation rendering.
![Scientific Visualization](https://github.com/raymondhernandez482/Scientific-Visualization-Lab/blob/a7ff8675c6169abca29e3b55f3760eac64c834e2/para%2012.jpeg?raw=true)
# Scientific Visualization Lab: 3D Scalar Field Analysis & Volumetric Rendering

![GitHub License](https://img.shields.io/badge/license-MIT-blue.svg)
![ParaView Version](https://img.shields.io/badge/ParaView-5.10+-orange.svg)
![Field](https://img.shields.io/badge/Field-Data_Science-green)

## 🔬 Project Overview
This repository showcases advanced data visualization techniques developed in the **Scientific Visualization Lab**. The primary focus is the interpretation of 3D scalar fields using **ParaView** to extract meaningful insights from complex datasets. By utilizing both volumetric and surface rendering, this project demonstrates how to identify spatial patterns, gradients, and periodic fluctuations within a defined Cartesian domain.

## 🖼️ Featured Visualization
![Scientific Visualization](https://github.com/raymondhernandez482/Scientific-Visualization-Lab/blob/a7ff8675c6169abca29e3b55f3760eac64c834e2/para%2012.jpeg?ra

## 🏆 Key Achievements & Technical Skills
* **Multimodal Data Representation:** Implemented side-by-side comparative analysis of Volumetric vs. Surface rendering.
* **Transfer Function Optimization:** Engineered custom opacity ramps to reveal internal "hidden" structures without losing spatial context.
* **Color Theory Application:** Applied divergent "Cool-to-Warm" color maps (Range: -3.2e+01 to 2.8e+02) to maximize visual contrast and data readability.
* **Spatial Analysis:** Configured 3D bounding boxes and coordinate grids for precise data localization.
## 🛠 Technical Breakdown
### 1. Volumetric Translucency (Left View)
* **Technique:** Ray-casting based Volume Rendering.
* **Utility:** Essential for "non-destructive" inspection of the dataset. By mapping scalar values to transparency, we identify high-density clusters at the base of the volume.
* **Key Insight:** Reveals the internal distribution of values that are typically obscured by the outer "skin" of the data.

### 2. Isosurface & Surface Mapping (Right View)
* **Technique:** Surface Rendering with Scalar Mapping.
* **Utility:** Highlights the behavior of the data at the boundaries.
* **Key Insight:** The orange-to-red oscillations at the upper boundary indicate a periodic frequency in the data source, captured here with high fidelity.
## 📦 Dependencies & Setup
To reproduce these results, ensure your environment meets the following requirements:
* **ParaView (v5.10 or higher):** Main rendering engine.
* **VTK (Visualization Toolkit):** For backend data processing.
* **Python 3.x:** (Optional) Used for automated state file generation via `pvpython`.
* **Hardware:** Recommended GPU with OpenGL support for real-time volumetric ray-casting.
## 🚀 Reproduction Steps
1.  **Initialize:** Load the dataset (e.g., `.vti` or `.vtk` format) into ParaView.
2.  **Volume View:** Set Representation to `Volume`. Open the `Color Map Editor` and modify the opacity curve to filter out low-value noise.
3.  **Surface View:** Create a layout split. Set Representation to `Surface`. 
4.  **Annotations:** Enable `Axes Grid` and `Orientation Widget` to maintain spatial reference across views.
## 📜 License
This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details. This makes the work open-source and professional for community contribution.
## 📬 Contact & Collaboration
I am passionate about turning complex data into actionable visual insights. 
* **GitHub:** [@raymondhernandez482](https://github.com/raymondhernandez482)

## Focus Areas
- 3D scientific datasets
- Simulation visualization
- Volume rendering
- Scientific data exploration
## Tools
ParaView
Python visualization libraries
Open scientific datasets

scientific visualization lab advanced three dimensional analysis and computational fluid dynamics modeling

![GitHub License](https://img.shields.io/badge/license-MIT-blue.svg)
![ParaView Version](https://img.shields.io/badge/ParaView-5.10+-orange.svg)
![Field](https://img.shields.io/badge/Field-Computational_Fluid_Dynamics-red)

🔬 Project Overview
Out here, you will find a collection of high-level science-based visuals. With ParaView doing the heavy lifting, raw numbers become clear images - especially through Volume Rendering and flow-line mapping. Think aerospace work, health sector imaging, even environmental systems - all lean on these methods heavily.

Stormy Workflow CFD Simplified
A single stream shows how liquid moves inside a shaped channel, drawn clearly with traced lines floating over a frame of thin edges. Visual details appear where motion meets structure, revealing paths shaped by walls. The view holds steady, guided by linked geometry and flow markers placed side by side without blending. Structure outlines stay visible beneath tracing patterns that follow movement step by step. Each line follows direction while mesh borders define space around it.

![Fluid Flow Visualization](https://github.com/raymondhernandez482/Scientific-Visualization-Lab/blob/a7ff8675c6169abca29e3b55f3760eac64c834e2/para%2013.jpg?raw=true)

🛠 Technical Highlights:
Through the data, flow lines took shape - revealing how speed and pressure shift across space. Inside the three-dimensional block, motion trends emerged without stating p outright. Paths bent where forces pushed hardest, drawn step by step. Volume details unfolded following invisible pushes. Gradients became visible - not labeled but shown through drift patterns. Movement traces followed pressure slopes like leaves on a current.
Through the wireframe view, a 3D grid appeared on top, helping check how tightly packed the lines were and whether they matched how air moves around surfaces. Shape of the mesh showed if spacing made sense where airflow changes fast or slows down near edges.
A sudden drop in pressure shows up as blue, then shifts toward red when fluid moves into the wider space. This color change marks where the current loops back on itself inside the chamber. Values span from negative point five zero seven to one point five zero across the area. The pattern reveals how the stream splits and folds near expansion points.

---

Project Two Ice Volume Measurement
A look inside how stuff spreads in three dimensions starts here. Density deep within takes center stage at first. Movement along outer layers follows close behind. One thing leads to another without rushing ahead.

![Scalar Field Visualization](https://github.com/raymondhernandez482/Scientific-Visualization-Lab/blob/a7ff8675c6169abca29e3b55f3760eac64c834e2/para%2012.jpeg?raw=true)

🛠 Technical Highlights:
Hidden layers came into view through specially shaped transparency rules. What once stayed buried now showed up in clear detail. A tailored approach made it possible to see beneath the surface. Structures that were invisible before began to appear. By adjusting how light passed through data, depth became visible. Details emerged where nothing could be seen earlier.
Floating layers next to dense slabs - watch how light slips through one but sticks in the other. Each rhythm in the numbers shows up clearer on one material than the second. Patterns breathe differently when space is filled versus when it’s carved. One method catches pulses the other tends to miss. What vanishes in solid forms often stands out in open volumes.
Hire Ready Technical Stack
Tools ParaView Primary VTK Python pvpython.
Flow paths show up through computer simulations. Shapes pop out when surfaces form at fixed values. Light beams trace through space to reveal hidden details. Grids bend as structures shift over time. Sections get removed so inner parts become visible.
Working often with .vti files, also some work using .vtk. Files like .stl come up regularly, while .vtu appears now and then. Each format handled without relying on defaults. Experience built through repeated use, not one-off tests. Tools adapted depending on file type. No preference shown toward any single extension.

Replication and Initial Configuration
Start by checking that ParaView version 5.10 or newer sits on your system.
Start things off by picking the `Stream Tracer` option - feed it a line or scattered points to kick the flow visuals into motion. From there, paths form where data moves, shaped only by how seeds are placed at the start.
Start by assigning the "p" value to either Rainbow Uniform or Cool-to-Warm settings - this brings out color shifts clearly. With these choices, gradients show up without confusion. Instead of mixing options, stick to one preset at a time. Clarity comes through consistent coloring. Finish when transitions look smooth across the range.

📜 License
This Project Uses The MIT License.
📬 Contact and Collaboration
Looking into jobs that mix data visuals with scientific computing tasks. My focus leans toward positions where numbers meet clear graphics. Work involving code and visual storytelling fits well. Opportunities showing real results through images interest me most. Roles letting me shape complex info into something viewable stand out.
GitHub: [@raymondhernandez482](https://github.com/raymondhernandez482)
LinkedIn profile link
