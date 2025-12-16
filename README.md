\# Full Fresnel – Blender Examples



This repository contains Blender scene files and assets accompanying the paper



> \*\*Enhanced Multispectral Rendering with a Unified Complex-Index Fresnel Model in Blender\*\*  

> P. T. Heerdt  

> \*to appear in\* \*\*The Visual Computer\*\*



The provided examples were used to generate figures in the paper and are intended to support 

reproducibility and inspection of the proposed method.



---



\## Repository Contents



\- `examples/`  

&nbsp; Blender scene files (`.blend`).  

&nbsp; Each example name refers to the corresponding \*\*figure number in the paper\*\*.



\- `assets/`  

&nbsp; HDRI environment maps used as scene illumination.



---



\## Full Fresnel Material Implementation



The Blender material shader implementing the \*\*full Fresnel model with a unified complex index of refraction\*\*, 

as described in the paper, is implemented in Blender’s source code and is \*\*not duplicated in this repository\*\*.



The relevant Blender source code modifications are available at:



https://github.com/PTHeerdt/blender-full-fresnel



These Blender scene files reference that material implementation and are intended to be used only with 

the above Blender build that includes the modifications.



The Blender scenes use relative paths to reference the provided HDRI environment maps in the assets/ directory.

The HDRIs should therefore not be added or re-linked manually after opening a scene, 

as doing so may break the relative path setup and lead to missing or duplicated environment textures.



---



\## Environment Maps and Licensing



All HDRI environment maps included in the `assets/` directory were downloaded from \*\*Poly Haven\*\*:



https://polyhaven.com/



Poly Haven assets are provided under the \*\*CC0 (public domain) license\*\*, allowing free use without attribution. Therefore, no copyright or licensing restrictions are violated by their inclusion in this repository.



---



\## Usage Notes



\- The repository uses \*\*Git LFS\*\* to store `.blend` files.  

&nbsp; To obtain the complete Blender scenes, Git LFS must be installed before cloning:

&nbsp; ```bash

&nbsp; git lfs install

&nbsp; git clone https://github.com/PTHeerdt/full-fresnel-examples.git

