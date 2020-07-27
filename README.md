Link to site: https://zachnguyen.github.io/Exoplanets-Visualization/

# Introduction

Not very long ago, the first people to discover exoplanets and jumpstart the hunt for worlds much like our own has [won the Nobel Prize for Physics](https://www.newscientist.com/article/2218951-nobel-prize-in-physics-for-discovery-of-exoplanet-orbiting-a-star/#:~:text=The%20Nobel%20prize%20in%20physics,Earth's%20place%20in%20the%20cosmos.!). 

Exploring distant worlds not only enhances our scientific knowledge, but also is fascinating in the own sense. It speaks to our common sense of curiosity and adventure into the unknown. In these times of pandemic and divisiveness, perhaps a common fascination of the universe will unite the human race regardless of gender, ethnicity or socio-economic background.

![](https://www.economist.com/sites/default/files/images/2018/10/articles/main/20181006_stp003.jpg)

As a data scientist and an astrophysics enthusiast myself, I want to do these findings justice by sharing two key visualizations. The purpose of this blog is to display the power of data visualization to illumninate some of the coolest things we have figured out while picking up some astrophysics knowledge on the way.

The data was collected through the API of [NASA's exoplanet archive](https://exoplanetarchive.ipac.caltech.edu/). It was modeled through python with the help of excellent open source data-viz engine like Bokeh and Plotly. 

Without further ado, let's arrive at our first visualization, a visualization through space ...

<iframe src="/images/Star_Coordinate_Viz_Norm.html" sandbox="allow-same-origin allow-scripts" width="100%" height="1000" scrolling="no" seamless="seamless" frameborder="0"> </iframe>

*Note: You can play around with the interactive 3D plot by zooming (mouse wheel), looking around (left mouse) or panning (right mouse). Reset camera to go back to default view and hover in for the finer details for each.

The plot shows a cartesian coordinate of the stars we have encountered which contain exoplanets in its systems. Some interesting points that we can learn from the plot are:
- The stars we've found exoplanets in are not very uniformly dispersed. If we've collected perfect data, this would mean something in the trend. Unfortunately, the non-uniform distribution is due to availability bias (We've only had the ability to look closely on a certain patches of the sky and not everywhere, therefore we didn't find exoplanets everywhere).
- The cluster that formed the clear columns of stars are the field vision of the Kepler Space Telescope (the one designed to find exoplanets among stars). In fact, we can see the sky path that Kepler was in charge of by reseting to default camera position, zooming in to maximum using your mouse wheel (you'll be in Earth's position), then looking around (left mouse). With a bit of luck, you should find a sky patch that looks like this:
![](https://supernovacondensate.files.wordpress.com/2012/07/kepler-set-7.jpg?w=700)
- According to the density of this cluster of the stars that contain exoplanets, we should expect exoplanets to appear as densely (basically everywhere) in every other direction we look. That's a good sign. This science is young and there is much to explore.
- I've coded the size of the marker for the radius of the stars (bigger size means bigger stars). By going to the default camera position, we can see that bigger stars don't appear in the Kepler cluster, but does everywhere else. The most likely reason for that is that we are more likely to find exoplanets in bigger star since we can observe them more closely for light dip (which shows periodic transit by planets) or gravitational anomaly (which shows that the star's path might be influenced by a planet with large gravity).
- I've also coded the color for star temperature with a diverging colorscale and normalize the star temperature to a 0-1 range. In this way, even though we miss out on the absolute temperature data (let's face it, it will be hell on Earth before we can intuit what 12,000K is like), we gain a clear relative comparison in the data (blueish markers are cooler than roughly 50% of all the stars whereas reddish markers are hotter than roughly 50% of all the stars). 
- We can learn here that larger stars are more likely to be cooler. This is because these stars have lived past their young and dangerous life, burning away their fuel incessantly. Now that they are no longer running fusion, they cool down and cause the gas to expand.

Write analysis here ...

<iframe src="/images/Pair-wise_exoplanet_characteristic.html" sandbox="allow-same-origin allow-scripts" width="110%" height="1000" scrolling="no" seamless="seamless" frameborder="0"> </iframe>

Write analysis here ...
