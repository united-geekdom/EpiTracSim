
# EpiTracSim: contact tracing simulator

`EpiTracSim` simulates the spread of an infection in a population of individuals, and evaluates the performance of a proposed contact-tracing method. For details of the method, see <A HREF="https://github.com/rsidd120/EpiTracSim/raw/master/Guttal_Krishna_Siddharthan_mobileriskfactor_20200426.pdf">manuscript</A> by Vishwesha Guttal, Sandeep Krishna, Rahul Siddharthan, "Risk assessment via layered mobile contact tracing for epidemiological intervention" (under processing at medRxiv).

Briefly: the idea is to assign to each individual in a population a probability of being infected. In common with other tracing methods, meeting an infectious individual changes your probability of being infected. However, so does meeting a probably infectious individual who has not been diagnosed. This chain of probabilities can go to any extent.  In addition, when an individual is tested and diagnosed positive or negative, all contacts of that individual are updated, as well as all contacts of contacts, and so on, recursively up until a pre-defined "tolerance". 

Right now this repository contains two files: EpiTracSim.jl which is a Julia module to be loaded into your own code, and a sample Jupyter notebook <A HREF="https://github.com/rsidd120/EpiTracSim/blob/master/EpiTracSim_demo.ipynb">EpiTracSim_demo.ipynb</A>, which you can click on to view within GitHub or load into your own Jupyter Julia session.  The code will be updated regularly. 
