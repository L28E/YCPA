# YCPA

2. Basic Simulation
    - `SoftSimpleReg.m` simulates a line source emitting a gaussian pulse which propogates through the region. In the region there is a box with high permittivity which the wave interacts with.
    - line 43 (`epi{1}(125:150,55:95)= c_eps_0*11.3;`) changes the permittivity of the inclusion. If we comment it out the wave is simply absorbed by the right boundary
    - `bc{1}.s(1)` sets up the source. As an example, if we change line 66 to `bc{1}.s(1).xpos = nx{1}/(2) + 1;` the line source is moved to approximately halfway along the x axis  
    - bc{1}.xm/xp/ym/yp changes the behaviour at the boundaries. Type 'e' seems to create an e field
3. Geometric Changes:
    - when the “st” paramater is set to -0.05 there seems to be a lot more reflections of the front face of the grate?
    - Changing the freq changes the wavelength 
4. Be creative:
    - Made a lil "C" shaped boxy thing