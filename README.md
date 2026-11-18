### About

---

This project is a CPU-based ray tracer written entirely in modern C++ using only the standard library. It was developed while working through Peter Shirley's *Ray Tracing in One Weekend* series, with the goal of better understanding how ray tracing works.

*Concepts*
- **Vector Mathematics** for ray generation, surface normals, and geometric calculations.
- **Ray-Object Intersections** to determine how rays interact with scene geometry.
- **Diffuse Scattering** using Monte Carlo sampling to simulate indirect lighting.
- **Material Systems** that model how different surfaces absorb, reflect, and transmit light.
  - **Metallic Reflection** with adjustable surface roughness.
  - **Dielectric Refraction** based on Snell's Law, including total internal reflection and Fresnel effects.
- **Gamma Correction** to account for nonlinear display response.
- **Anti-Aliasing** through stochastic supersampling to reduce square edges.
- **Depth of Field** produced by modeling a camera aperture and focal distance.
- **Recursive Path Tracing** where rays bounce through the scene, accumulating light contributions until termination.
- **Motion Blur** produced by simulating time during the shutter window.

While the renderer follows the layout given by the series, the primary focus of this project was building an understanding of the underlying concepts of ray tracing.

Pictures
---
![First Sphere](images/FirstSphere.jpg)

*First sphere rendered in this project. Colors mapped relative to the spheres normal vectors.*

![Diffuse Sphere](images/DiffuseSphere.jpg)

*Introduction of diffuse light scattering using random ray sampling, along with gamma correction to improve perceived brightness.*

![Sphere Materials](images/SphereMaterials.jpg)

*Implementation of a material system supporting multiple surface behaviors within the same scene.*

![Glass Sphere](images/GlassSphere.jpg)

*Dielectric material demonstrating refraction, reflection, and a hollow glass sphere containing an internal air pocket.*

![Different Perspective](images/Perspective.jpg)

*Refactoring of the camera system into a reusable component, allowing flexible scene composition and camera positioning.*

![Depth Of Field](images/DepthOfField.jpg)

*Simulation of a finite camera aperture to produce realistic depth of field effects and focus blur.*

![Large Scene](images/LargeScene.jpg)

*Large Scene with each sphere containing a randomly assigned material.*
