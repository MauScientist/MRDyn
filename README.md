![Imagem_1](https://github.com/user-attachments/assets/2f79925e-4a9d-4251-979a-44fbb106c7c3)


For better performance of the created scripts we indicate:

[![Blog](https://img.shields.io/badge/Julia%20Lang-Download-red?style=for-the-badge)](https://julialang.org/)
[![Blog](https://img.shields.io/badge/Ubuntu-Download-orange?style=for-the-badge)](https://www.ubuntu.com)
[![Blog](https://img.shields.io/badge/Python-Download-blue?style=for-the-badge)](https://www.python.org)


The Olivia Dynamics (ODyn) consists of scripts in Julia and Python language for the analysis of non-linear dynamic systems. The scripts that make up the ODyn calculate the Lyapunov Exponents, Bifurcation Diagrams, 01-Test and Basins of attraction, Portrait Phase and Poincare Map, thus forming a diagnosis of the chaotic or periodic behavior of the analyzed nonlinear dynamics system.

Access to repository in 


[![Blog](https://img.shields.io/badge/Repository-Download-red?style=for-the-badge)](https://github.com/ScienceMau/Olivia-Project)


## Installation

### Linux
- Ubuntu
For installation in particular use the command: `sudo snap install julia -classic`


 ### Windows
For installation on Windows systems, just download from <a href="https://julialang.org/">HERE</a> the .exe for the system Windows operating system and follow the steps indicated by the app. And then click on the icon on your Desktop and install the libraries. To do so, just type in Julia's terminal: `using Pkg; Pkg.add("Package Name");`

### Packages

For its use it is necessary to install the following packages:
<ul>
<li><a href="https://docs.julialang.org/en/v1/manual/distributed-computing/">Distributed</a></li>
<li><a href="https://juliadynamics.github.io/DynamicalSystems.jl/dev/">Dynamical System</a></li>
<li><a href="https://docs.julialang.org/en/v1/stdlib/SharedArrays/">SharedArrays</a></li>
<li><a href="https://github.com/JuliaIO/MAT.jl">MAT</a></li>
<li><a href="https://docs.julialang.org/en/v1/stdlib/Statistics/">Statistics</a></li>
<li><a href="https://github.com/SciML/OrdinaryDiffEq.jl">OrdinaryDiffEq</a></li>
 <li><a href="https://docs.julialang.org/en/v1/stdlib/DelimitedFiles/">DelimitedFiles</a></li>
</ul>

- For installation use code in prompt julia:

```
using Pkg
v = ["DynamicalSystem","SharedArrays","Statistics","OdinaryDiffEq","DelimitedFiles"]
for i in v
  Pkg.add(i)
 end 
```

## Codes 

### Dynamical Analisys (In Julia)

1. **MathModel.jl** : Script to write first order differential equations, parameters and initial conditions.
2. **Lyapunov.jl**: Script that calculates Lyapunov exponent and bifurcation diagram
3. **Phase_portrait_and_poincare_map.jl**: Script that builds Phase Portrait and Time Series
4. **Basins.jl**: Script that calculates the Basins of attraction of system.
5. **Test-01.jl**: Script that calculates the 01-Test.

### Plots (In Python)

1. **Lyapunov_and_bifurcation_plot.py** 

Example of result obtained with the Lyapunov.jl e Lyapunov_and_bifurcation_plot.py

![bif_lyapunov_intermitent](https://github.com/ScienceMau/Olivia-Project/assets/61286097/9fbe9b7a-a7d8-4666-a75f-b6442382d7d3)


2. **Basins_and_attractors_plot.py**

Example of result obtained with the Basins.jl and basins_and_attractors_plot.py

![bacia_atracao_casimir](https://github.com/ScienceMau/Olivia-Project/assets/61286097/4e39997c-bb46-45e3-a99f-b20e60e9f072)

3. **Phase_portrait_and_poincare_map_plot.py**

Example of result obtained with the Phase_portrait_and_poincare_map.jl and Phase_portrait_and_poincare_map_plot.py

![poincare_TS_intermitent](https://github.com/ScienceMau/Olivia-Project/assets/61286097/3a175736-b2ba-4a8d-bfa1-b2bd5f4cbb6b)



## Publications:

1. Ribeiro, Mauricio A.; Jose M. Balthazar, Ângelo M. Tusset, Átila M. Bueno, and Hilson H. Daum. 2022. ‘MEMS-Based Atomic Force Microscope: Nonlinear Dynamics Analysis and Its Control’. Vibration Monitoring and Analysis - Recent Advances [Working Title]. IntechOpen. doi:10.5772/intechopen.108880.

2. Ribeiro, Mauricio A.; Jose M. Balthazar, Hilson H. Daum, Angelo M. Tusset (In Press). 'Nonlinear Dynamics Behavior and Its Control under Frequency-Varying Excitations for Energy Harvesting'. International Journal of Nonlinear Dynamics and Control

3. Ribeiro, Mauricio A., Angelo M. Tusset, Wagner B. Lenz, José M. Balthazar*, Grzegorz Litak; On non-linear dynamics behaviour of a fixed offshore platform for energy harvesting. 16th INTERNATIONAL CONFERENCE Dynamical Systems – Theory and Applications December 6-9, 2021 (On-line)





Essa suite de códigos é utilizada para analisar sistemas dinâmicos não lineares considerando o ferramental clássico. Essas analises permitem diagnosticar o comportamento de caos no sistema de equações diferenciais que descrevem o fenômeno a ser estudado.
Os scripts são inteiramente escritos em Julia Lang com o auxílio de algumas bibliotecas que podem tornar a analise mais fácil de ser programada. Como resultado os scripts retornam um .dat que possui os dados calculados para se tornarem gráficos em seu software de preferência. Nós iremos disponibilizar também alguns scripts em Python usando a Matplotlib e Numpy para pode confeccionar seus gráficos com os resultados. Como um resultado prévio os scripts em Julia Lang tbm retornam arquivos .png para uma observação prévia.

