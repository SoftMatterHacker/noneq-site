+++
date = "2017-01-22T13:35:16+11:00"
draft = false
title = "ImageJ - touching circles"
tags = ["wiki","imagej","particle"]
math = true
image = ""

+++
Image processing saves a LOT of time in your research, but we can't always rely on the 
default menu choices to do everything, even in fantastic software like [ImageJ](https://imagej.nih.gov/ij/).  One need
of microfluidics researchers is the separate size analysis of spherical (circular in 2D) droplets that
are very similar in size but are mostly touching.  

Most image analysis approaches require you to have separate particles in your sample before they can be
automatically identified during processing, so to analyze an image like the one below we need to perform some extra 
pre-processing steps.

{{< figure src="/img/circles1.png" title="Starting image of droplets, made by Zengyi Wei." >}}

The first step is to make the image 8-bit using: Image->Type->8-bit:
{{< figure src="/img/circles2.png" title="Grayscale image converted from above." >}}

Then binarize the image using Image->Adjust->Threshold:
{{< figure src="/img/circles3.png" title="Binary image of circles." >}}

Now invert the image using: Edit->Invert:
{{< figure src="/img/circles4.png" title="Inverted image" >}}
What we've done is essentially create black circles inside the white borders of the original drops.  
Now we have a clear boundary between particles.
This also creates 'particles' in between the circles, but we can deal with this in the next step.

Run Analyze-Particles with the parameters shown in the image (the key one seems to be a high minimum 
circularity, which is very selective for circles and avoids the interstitial shapes that are very non-circular):
{{< figure src="/img/circles5.png" title="Analyze those circles!" >}}

ImageJ finds the below circles, they are undersized because it ignores their wall thickness, 
but if you are focused on the polydispersity of the distribution this won't matter as much.
You could easily post-correct the under-estimate because you know the pixel size of the border that is ignored.
It misses a few, so feel free to tweak my settings:
{{< figure src="/img/circles6.png" title="Found most of them!" >}}

