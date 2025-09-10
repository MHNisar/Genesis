# Genesis
Portfolio Longevity in Contemporary Markets


Brief Description for each Sheet:
Historical:
This sheet houses the foundational dataset for the simulation. It contains annual historical returns for stocks, bonds, and inflation, along with the calculated correlation between asset classes for each year. The model samples randomly from this data to generate stochastic return sequences.
Control:
This sheet contains all user-defined parameters to run the simulation, including the starting portfolio balance, asset allocation (stock/bond weights), withdrawal rate, and the range of historical years to sample data from.         
r1:
The core computational sheet. It runs a single, randomized 30-year retirement scenario by drawing sequences of returns and inflation from the historical data. It calculates the annual portfolio value, withdrawals, and adjusts for inflation, providing a detailed look at one potential outcome.
Simulations:
This sheet summarizes the outcomes from running thousands of simulations.

Note: Please enable VBA applications for the model by right-clicking on the downloaded file > Properties > General > Unblock



