# Ocean Simulation

Developed in C++ and OpenGL, this real-time simulation uses the Fast Fourier Transform method (FFT) to simulate waves, inspired by the paper ["Simulating Ocean Water"](https://people.computing.clemson.edu/~jtessen/reports/papers_files/coursenotes2004.pdf) by Jerry Tessendorf. Additionally, it is parallelized using OpenCL and employs Physically-Based Rendering (PBR) and image-based lighting (IBL) techniques to enhance the realism of the oceanic visuals, and an HDR skybox to present dynamic and an immersive sky. 



## Features

#### Physically-Based Rendering (PBR)

PBR techniques are employed to simulate realistic material properties. This approach ensures that the water surface in the simulation accurately reflects and refracts light, mimicking the way light interacts with natural water. The result is a stunningly realistic depiction of the ocean, complete with nuanced lighting effects.



#### Image-Based Lighting (IBL)

To further improve visual fidelity, Image-Based Lighting (IBL) is used. This technique utilizes real-world imagery to provide environmental lighting, ensuring that the simulation's lighting conditions are based on actual atmospheric lighting. This results in richer reflections and more accurate illumination across the simulated ocean.



#### Ocean Waves using Fast Fourier Transform (FFT)

The Fast Fourier Transform (FFT) algorithm is used to simulate realistic ocean waves. This mathematical approach is inspired by Jerry Tessendorf's paper ["Simulating Ocean Water"](https://people.computing.clemson.edu/~jtessen/reports/papers_files/coursenotes2004.pdf). The FFT algorithm creates dynamic, lifelike wave patterns that faithfully mimic real oceanic conditions.



#### Phillips Spectrum for Wave Energy Modeling

The simulation incorporates the Phillips Spectrum, a mathematical model that provides a detailed statistical representation of wave energy distribution. By using this model, the simulation can accurately depict the varying energy levels across different wave frequencies, adding to the authenticity of the ocean wave behavior.



#### Dynamic HDR Skybox 

An HDR (High Dynamic Range) Skybox is introduced to present a more dynamic and immersive sky. This feature captures the vast range of luminance of real-world skies, from the brightest clouds to the darkest nights, creating a more lifelike backdrop that enhances the visual experience.



#### Atmospheric Fog

Atmospheric fog effects are implemented to add depth and a captivating ambiance to the scene. This contributes to the visual appeal of the simulation and adds a layer of realism by mimicking the way fog interacts with light and the environment in natural settings.



#### Infinite Ocean

The Infinite Ocean feature ensures that the ocean landscape extends endlessly, providing a consistent and immersive backdrop. This feature is crucial in creating a believable and boundless oceanic environment, where the horizon seamlessly meets the sky, just like in the real world.



#### Frustum Culling

This simulation uses frustum culling to optimize the performance of the simulation. By rendering only the elements that are within the player's field of view, it significantly reduces the processing load. This optimization ensures smooth and responsive performance, even when rendering complex scenes.



#### OpenCL Parallelization

The library OpenCL is used to parallelize the FFT computation for waves simulation, by utilizing the GPU and the CPU for maximized speed and efficency. This greatly enhances the overall performance and responsiveness of the simulation.



#### Adjustable Ocean Temperament Settings

Users have the flexibility to adjust the ocean's temperament in the simulation. This feature allows for a seamless transition between calm, serene waters and more turbulent, stormy seas, offering a varied and interactive experience.



## License

This project is licensed under the Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License.  
[Read the full license here](https://creativecommons.org/licenses/by-nc-nd/4.0/).

## Installation

1. Clone the repository:
```
git clone https://github.com/AmrHMorsy/ocean_simulation-.git
```
2. Navigate to the project directory: 
```
cd Ocean_Simulation
```
3. Create a build directory: 
```
mkdir build
```
4. Navigate to the build directory: 
```
cd build
```
5. Generate makefiles using cmake: 
```
cmake ../
```
6. compile using makefile: 
```
make
```
7. Run the program: 
```
./ocean_simulation
```
<br>
