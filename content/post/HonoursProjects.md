+++
title = "2020 Honours Project Descriptions"
date = 2019-07-20
draft = false

# Tags and categories
# For example, use `tags = []` for no tags, or the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags = []
categories = []

# Featured image
# Place your image in the `static/img/` folder and reference its filename below, e.g. `image = "example.jpg"`.
# Use `caption` to display an image caption.
#   Markdown linking is allowed, e.g. `caption = "[Image credit](http://example.org)"`.
# Set `preview` to `false` to disable the thumbnail in listings.
[header]
image = ""
caption = ""
preview = true

+++
### Note: As of 2020, all Honours projects are literature- or simulation-based only.  We can not support experimental projects, so please be aware that working with us will not likely involve ANY lab time. 

Below are our current projects:

1. **Research question: What shape is best for biological interfacing?**
  * **Problem Statement:** Numerous biological processes involve purely physical interactions dictated by the shape of two surfaces or entities. An example is phagocytosis, when white blood cells engulf invading cells but struggle to ingest particles that are too long and narrow. Another example is plant pollination, where particles with uniquely irregular shapes match up with complementary plant surfaces. How do we draw on nature's examples and construct design laws for new shapes that can control biological and medical mechanisms?
  * **Literature background:** Example articles (and their references) include the work by [Champion](https://www.pnas.org/content/103/13/4930.short), [Ruiz-Herrero](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.123.038102), and [Skotheim](https://science.sciencemag.org/content/308/5726/1308).
  * **Project deliverables:** 
        1. Survey the literature in various natural areas, and identify other shape-based mechanisms.
        1. Link the observed mechanisms by identifying commonalities, like limiting curvatures, key length scales, and physical properties.
        1. Map the behaviors and point out where gaps exist that aren't physically prohibited.
{{< figure src="/img/daisys.png" title="Spiky pollen grains." >}}     

2. **Research question: What structures form during aggregation of complex, restructuring droplet shapes?**
  * **Problem Statement:** The formation of colloidal gels, by aggregation of attractive particles or droplets into fractal networks, is a key mechanism of structure formation in numerous materials. Simulations of fractals made from spherical building blocks are widely available, but little work exists on more complex systems with non-spherical shapes that undergo restructuring. Shaped materials are the future of structure and performance control, and we need to be able to predict their assembly.
  * **Literature background:** Get started by reading about [fractal sphere gels](https://link.springer.com/article/10.1023/A:1008731904082), fractal [rod gels](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.92.155503), arrested coalescence of [ellipsoidal droplets](https://pubs.acs.org/doi/abs/10.1021/acs.langmuir.8b02136), and the modeling of restructuring fractal droplet gels.
  * **Project deliverables:** 
        1. Code a simulation of fractal aggregation of spheres, then modify to incorporate rods.
        1. Use more recent work to modify the code to allow the rods to restructure according to physically realistic rules.
        1. Determine the range of structures formed and contrast with past work on restructuring systems.
        1. Explore the effects of sub-unit size on structure.
{{< figure src="/img/40paraff.png" title="Fractal droplet network." >}}      
        
3. **Research question: How can shape be used to design and control active matter particles?**
  * **Problem Statement:** Physicists have found fascinating behavior in living systems where large numbers of participants, like bacteria and flocking birds, can exhibit collective patterns of movement without the need for complex rules, a field in physics called *Active Matter*. This is important, as it means quite complex behavior can be simulated using relatively simple rules. New models will enable us to design active particles to mimic complex biological functions for drug delivery.
  * **Literature background:** Read up on [active matter](https://www.annualreviews.org/doi/full/10.1146/annurev-conmatphys-070909-104101), then methods of its [simulation](https://journals.aps.org/rmp/abstract/10.1103/RevModPhys.85.1143).
  * **Project deliverables:** 
        1. Code a simulation of active particles inside of a polymer gel when the particles diffusively release an enzyme that degrades the surrounding polymer network. 
        1. Simulate the movement of the particles inside polymer gels with different degrees of cross-linking and density.
        1. Modify the simulation to consider particles with anisotropic shapes, allowing directional bias.
        1. Modify the particle behavior so that the enzyme is immobilized inside, ensuring reaction occurs only at the particle surface.

{{< figure src="/img/wiggles.png" title="Tracks of active particles on the move." >}}


