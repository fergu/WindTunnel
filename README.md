# WindTunnel
 A simple potential flow "wind tunnel" for flow around a cylinder (mapped to a wing) written in javascript.

This code solves the potential flow around a cylinder and then uses a conformal mapping technique to map the solution on the cylinder to one surrounding an airfoil. Given the solution's underpinnings as a potential flow solver this means that it is subject to all of the caveats that come with obtaining a potential flow solution. Most notably, this flow is inviscid, irrotational, and incompressible. There are no boundary layers, separation, or other things you might intuitively expect.

This project was very much conceived as a sort of "hands on" demonstration for young hopeful-scientists and engineers, not as any sort of overly-accurate representation of the fluid mechanics involved. It is, of course, as accurate as you would expect any potential flow solution to be for flow around a wing.

Fluid flow is a hard thing to conceptualize given that we can't see it, and the goal of this simulation is to help give a mental picture of what is happening when a wing moves through the air. For example, there's this common misconception that the reason wings produce lift is because the air that goes over the top of a wing needs to 'keep up' with its counterpart on the bottom. Try that out here, and you might learn that this is just not true!

Each "smoke particle" in this simulation is colored by its velocity (which is in turn related to pressure). The more red a particle turns the faster it is going and the lower its (static) pressure will be according to Bernoulli's principle. You might notice that the smoke that goes over the top of a wing tends to to get more red than that which goes below - this is the reason wings produce lift! The reasons "why" air over the top of a wing goes faster than the bottom are a bit more complex, but come down to the influence of the wing on the surrounding air ("turning" the air to follow the wing surface, thus changing the fluid velocity and therefore pressure and lift), but this in turn causes an influence on the wing by the air, and so on! 

I am working on a version of this simulation which uses OpenGL web shaders to produce a more realistic simulation. Keep an eye out!
