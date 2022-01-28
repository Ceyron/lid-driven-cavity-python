# Computational Fluid Dynamics in Python

![lid-driven-cavity](https://user-images.githubusercontent.com/27728103/151614448-947d4ac8-fa4a-40f6-b0e1-04baf18eee87.gif)

Using NumPy to solve the equations of fluid mechanics  🌊🌊🌊 together with Finite Differences, explicit time stepping and Chorin's Projection methods.

You can find more details in the [corresponding video](https://youtu.be/BQLvNLgMTQE) which you can also use to code along 👩‍💻. More scripts like this can be found [in this GitHub Repo](https://github.com/Ceyron/machine-learning-and-simulation).

## How to use

Make sure you have the relevant packages installed. These pip commands should be sufficient

    pip install numpy matplotlib tqdm

Then you can either execute

    python lid_driven_cavity_python_simple.py

for a simulation which runs all the way through and in the end plots a contour plot of the (pseudo) pressure with a vector field layed on top. Or you can execute

    python lid_driven_cavity_python_simple_interactive_plotting.py

to get a simulation that plots throughout time. By this you can see how the Lid Driven cavity is reaching its steady-state.

## Parameters

In the beginning of both files, directly after the explaining docstring, you find Python constants to adapt the scenario and the numerics.

## Details on the methods

The method is based on the [operator splitting due to Chorin](https://math.berkeley.edu/~chorin/chorin68.pdf). Also see [this](https://en.wikipedia.org/wiki/Projection_method_(fluid_dynamics)) Wikipedia page for some details.

Big parts of the of the code, including the approach to solve the pressure-poisson equation using Jacobi Smoothing, are inspired by the [11th lesson](https://nbviewer.org/github/barbagroup/CFDPython/blob/master/lessons/14_Step_11.ipynb) of Lorena Barba's 12 steps to Navier Stokes.

Also check out the docstring in the beginning of the file for some more details.