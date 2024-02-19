# Parking Incentive Allocation for Ridesharing Systems
Data used in the paper "A Parking Incentive Allocation Problem for Ridesharing Systems".
The following describes the columns contained in each files. 

drivers.csv: information about drivers.
- origin: (longitude, latitude) coordinates of drivers' origin.
- destination: (longitude, latitude) coordinates of drivers' destination.
- purpose: Purpose of trips.
- trip_length: The distance between the origin and destination, computed by Haversine formulae.
- i: Index of drivers.
- arr_period: Arrival period of drivers ($t_i^\mathrm{arr}$).
- dep_period: Departure period of drivers ($t_i^\mathrm{dep}$).
- parking_periods: Parking periods of drivers.
- Ki: Set of parking periods for drivers ($K_i$).
- pi0: Probability of acceptance in case of not being offered an incentive.
- lenK: Indicate whether the driver is included in the configurations with the number of parking lots equals 1, 5, 20, respectively.

gamma.csv: Value of $\gamma_i$ parameters corresponding to different values of the promotion parameter.
- i: Index of drivers.
- promotion: value of the promotion parameter.
- gamma: value of $\gamma_i$.

theta.csv: Values of $\theta_i$ corresponding to different values of the revision parameter.
- i: Index of drivers.
- revision: value of the revision parameter.
- theta: value of $\gamma_i$.

realizations.csv: realizations of matches' result.
- i: Index of drivers.
- promotion: Value of the promotion parameter.
- rid: Index of the realization.
- is_suc0: Boolean, set to TRUE if the match result is successful when the incentive is not offered.
- is_suc1: Boolean, set to TRUE if the match result is successful when the incentive is offered.

parking.csv: information of parking lots corresponding different values of the capacity parameter.
- lenK: Indicate whether the driver is included in the configurations with the number of parking lots equals 1, 5, 20, respectively.
- capacity: Value of the capacity parameter.
- k: Index of parking lots.
- num_spaces: Number of spaces in parking lots.
- location: (longitude, latitude) coordinates of parking lots.
