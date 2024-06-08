# Jonathan Oppenheim's postquantum theory of classical gravity
Jonathan Oppenheim's postquantum theory of classical gravity offers a novel approach to the problem of unifying quantum mechanics and general relativity. Instead of quantizing gravity, as is done in traditional approaches like string theory or loop quantum gravity, Oppenheim's theory maintains gravity as a classical field while allowing for quantum matter fields to interact with this classical gravity in a fundamentally stochastic manner.

Oppenheim's model avoids the inconsistencies faced by the semiclassical Einstein equation, which attempts to describe quantum fields on a fixed classical spacetime background. His approach integrates classical gravity with quantum field theory by ensuring that the interaction remains consistent with the principles of both quantum mechanics and general relativity. This involves modifications to the quantum dynamics, making them fundamentally stochastic, which allows for a backreaction of quantum fields on the classical spacetime metric

# Postquantum Theory of Classical Gravity by me (mmtmn)

This project implements a simulation inspired by Jonathan Oppenheim's hypothesis on the postquantum theory of classical gravity. The code, created by mmtmn, simulates the interaction of quantum systems with classical gravity using OpenGL for visualization and OpenMP for parallel processing. The simulation includes 10,000 quantum systems that exhibit stochastic spacetime fluctuations, gravitational interactions, and decoherence, thereby exploring the theoretical framework where classical gravity interacts with quantum matter.

The simulation initializes a set of quantum and classical systems with random positions and velocities, then applies various physical processes including spacetime fluctuations, stochastic curvature fluctuations, and gravitational interactions. The systems' evolution is visualized in real-time, demonstrating how quantum systems decohere due to their interaction with the classical gravitational field, and how energy conservation is managed throughout the simulation. This project serves as both a conceptual exploration and a visual demonstration of the proposed theory's dynamics.

# Images

![image](https://github.com/mmtmn/Postquantum-Theory-of-Classical-Gravity/assets/42742390/73f0bd55-7243-4e32-921b-2921311bf1f9)
![image](https://github.com/mmtmn/Postquantum-Theory-of-Classical-Gravity/assets/42742390/18b5cd3d-bfbd-46e0-85af-fa990d80bdf6)
![image](https://github.com/mmtmn/Postquantum-Theory-of-Classical-Gravity/assets/42742390/499f7842-68af-4195-8d10-65e92fe98a2e)
![image](https://github.com/mmtmn/Postquantum-Theory-of-Classical-Gravity/assets/42742390/d24c421c-881b-49bf-9ade-da997f7fd38c)

# Controls
- 'a' moves to the left
- 's' moves backwards
- 'w' moves forward
- 'd' moves to the right
- move your cursor (pc's mouse or touchpad) to move the camera around

# How to change the code to run bigger or smaller simulations
- #define NUM_QUANTUM_SYSTEMS 1000 <-- change this number to achieve the results according to the capacity of your computer 


# Compile and run the code:

### Ubuntu/Debian-based Linux

1. Install necessary libraries:
   ```
   sudo apt-get update
   sudo apt-get install freeglut3 freeglut3-dev libglu1-mesa-dev build-essential
   ```
2. Compile the code:
   ```
   gcc -o main main.c -lGL -lGLU -lglut -lm -fopenmp
   ```
3. Run the program:
   ```
   ./main
   ```

### Fedora/RPM-based Linux

1. Install necessary libraries:
   ```
   sudo dnf install freeglut-devel mesa-libGLU-devel gcc gcc-c++
   ```
2. Compile the code:
   ```
   gcc -o main main.c -lGL -lGLU -lglut -lm -fopenmp
   ```
3. Run the program:
   ```
   ./main
   ```

### Arch Linux

1. Install necessary libraries:
   ```
   sudo pacman -S freeglut glu gcc
   ```
2. Compile the code:
   ```
   gcc -o main main.c -lGL -lGLU -lglut -lm -fopenmp
   ```
3. Run the program:
   ```
   ./main
   ```

### Windows (using MinGW)

1. Install MinGW and MSYS2 from the MinGW website.
2. Install necessary packages using MSYS2 shell:
   ```
   pacman -S mingw-w64-x86_64-freeglut mingw-w64-x86_64-gcc
   ```
3. Compile the code:
   ```
   gcc -o main main.c -lglut32 -lopengl32 -lglu32 -lm -fopenmp
   ```
4. Run the program:
   ```
   ./main.exe
   ```

### macOS

1. Install Xcode command line tools:
   ```
   xcode-select --install
   ```
2. Install Homebrew if not already installed:
   ```
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```
3. Install necessary libraries using Homebrew:
   ```
   brew install freeglut
   ```
4. Compile the code:
   ```
   gcc -o main main.c -framework OpenGL -framework GLUT -lm -fopenmp
   ```
5. Run the program:
   ```
   ./main
   ```
