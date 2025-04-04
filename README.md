# Mathematically Modeling the Environmental Effects of High-Performance Computing

With great “power” comes great responsibility. In recent years, the world has seen a massive increase and
progression of high-powered computing (HPC). Now a critical component in AI industries, the rise of HPCs
signifies a new area of mass energy consumption, which can lead to serious environmental impacts. In this
paper, we introduce a multi-step environmental impact model to evaluate the effects of HPC on the
environment, apply and adapt our model to various scenarios, and develop a set of recommendations to
mitigate these impacts along with a proposal letter to the United Nations Advisory Board to urge for more
emphasis on their consideration towards high-powered computing.

First, we collect data from two different datasets, one with a more narrowed scope (TOP500), and one with
an inclusive and broad scope (a global data center energy consumption dataset). We preprocess our data using
methods such as linear interpolation and grouping by average. We utilize Holt’s linear trend method to forecast
values for TOP500 which considers the futuristic growth of HPC. We leverage the geographical region
consideration, including North America, Asia, and Europe, from TOP500 and scale the quantities by a dataset
ratio derived with our second dataset to obtain more accurate global HPC environmental impacts. From our
data, we notice that HPC capabilities will utilize around 362 TWh of electricity in 2024, and a forecast of
1593 TWh in 2030.

To build our HPC environmental impact model, we first account for a dynamical energy mix by developing
a recursive function model based on our logistic function for renewable energy growth. We distinguish
energy mix ratios between each geographical region to provide a more realistic approach to these regions'
varying energy source priorities. Next, we develop a multivariate carbon emissions model and leverage our
dataset ratio to consider all data centers worldwide. Finally, to compose a clearer definition of environmental
impact, we include two environmental factors in our model: temperature impact and air quality impact. We
build our temperature impact model based on the theory of radiative forcing, and our air quality impact model
based off pollutant mechanisms. After constructing our model, we analyze the strengths and limitations. We
later expand on our HPC environmental impact analysis by developing a new model for HPC data center land
usage using a U.S. data center dataset, developing a relationship between power usage and land usage. We
test polynomial, linear, and logarithmic regression and use R2 metrics to choose our best-fit.
Next, we apply our models to a variety of different scenarios. We use our model to analyze the increase in
energy demand from other sectors by adding a cost parameter to model the increase in energy costs. We
notice that higher costs for certain energy sources due to demand slow their growth in energy mixes, eventually
reaching a dropping threshold where our model emphasizes priority over other energy sources. We then use
our model to forecast the impacts of HPC on the environment in 2030, creating a best-case and worst-case
scenario to provide realistic bounds. Furthermore, we analyze the case of increasing the portion of
renewable energy composition, measuring the carbon emissions reductions from 25% to 50% to 75% to 99%
renewable energy composition along with addressing the possibility of a 100% composition. Lastly, we use
our findings to create a set of recommendations to mitigate the environmental impact of HPC and draft a
proposal letter to the United Nations Advisory Board to urge for more emphasis on their consideration towards
high-powered computing.
