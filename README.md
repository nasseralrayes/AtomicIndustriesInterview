# AtomicIndustriesInterview

## Question 1
### Outlier part geometry identification
As you can imagine, there are lots of different shapes and sizes of plastic parts and injection mold components. We need to make sure all our software is robust to any geometry that a customer might throw at us. One component in handling our data is to automatically recognize and flag any geometric complexities that we haven’t previously dealt with and may cause issues. Imagine a simplified example, where our product has been finely tuned to function well on more simple geometries like cubes and spheres, typically referred to as primitives. In an ideal world, our customers would only provide us cubes and spheres, but unfortunately for us, that isn’t the case and we’d like some sort of middleware algorithm that can identify when customer parts are out of the ordinary.  Given a dataset of parts, we’d like you to design an algorithm capable of loading geometries and identifying whether the part is close to a simple primitive shape like a sphere, cylinder, square, etc. or if it is a more complex design that may require manual intervention or some additional layer of business logic.

We’d like you to create a proof-of-concept algorithm that is capable of addressing the problem statement above. The details of how to implement this is at your discretion. What we require is for you to provide us with the ability to evaluate and test your implementation. An example of this would be writing a python script that could be executed via the command line.
 
Note: The part files are in GMSH format (.msh) - we don’t expect you to be familiar with this file type so we’ve also included some example code and documentation that shows how to read in the files and get meaningful information out of them. You can also download the Gmsh desktop app to preview each part in the dataset.

The example code and part dataset can be found in this repository: https://github.com/Atomic-Industries/swe-interview 

## Question 2
### System design
Given your proof-of-concept, think about how you might implement a larger system that runs as part of our pre-processing pipeline. Every time new geometry comes into the system, we want to process it through a number of stages including your algorithm, storing it alongside any useful metadata and warning us of any potential problems. Please prepare 1 or 2 slides describing how you’d architect a system that processes large amounts of new part geometry as it streams into our dataset. Feel free to describe specific technologies that you’re familiar with, or just a general overview about how such a system might work.

