# Neutron Star Structure Simulation

This project simulates the theoretical structure of a neutron star using structural equations of state (EoS) and the Tolman-Oppenheimer-Volkoff (TOV) equation. The Python code computes the mass, radius, pressure, and energy density of a neutron star, using different EoS models.

## Project Overview

Neutron stars are incredibly dense stellar remnants that are typically formed when massive stars collapse. This simulation models the relationship between various parameters such as mass, radius, pressure, and energy density under hydrostatic equilibrium. Two different models are implemented in this simulation:

1. **Tolman-Oppenheimer-Volkoff (TOV) equation**: For relativistic conditions.
   $$\frac{dp}{dr} = - \frac{G \epsilon(r) m(r)}{c^2 r^2} \left( 1 + \frac{p(r)}{\epsilon(r)} \right) \left( 1 + \frac{4 \pi r^3 p(r)}{m(r) c^2} \right) \left( 1 - \frac{2 G m(r)}{c^2 r} \right)^{-1}$$

2. **Classical equation**: For non-relativistic conditions.
   $$\frac{dp}{dr} = - \frac{G \epsilon(r) m(r)}{c^2 r^2}$$

The results are visualized through plots of:

- Mass vs. Radius
- Pressure vs. Radius

Additionally, the simulation saves the computed data to an Excel file (`neutron_star_simulation_results.xlsx`).

## Requirements

To run the simulation, you'll need the following Python libraries:

- `NumPy`
- `Matplotlib`
- `Pandas`

You can install them by running:

```bash
pip install numpy matplotlib pandas
```

## How to Run Locally

1. **Clone the repository or download the code**.
2. **Run the Python script**:
   ```bash
   python simulation.py
   ```
3. **Choose a model**: The program will prompt you to choose between the "TOV" model or "Classical" model for the simulation. Type `TOV` for the relativistic model or `Classical` for the non-relativistic model.
4. **View the results**: After the simulation completes, two plots will be generated showing mass vs. radius and pressure vs. radius. You will also see a printout of the final results in the terminal, and the data will be saved to `neutron_star_simulation_results.xlsx`.

## Example Output
```bash
Final Results:
Energy Density = 2.62e35 N
Radius = 10545.41 m
Mass = 1.82 M0
Pressure = 1e35 N/m^2
```

## Example of Plots obtained

#### Theoretical curves of mass versus radius, and pressure versus radius -
![image](https://github.com/user-attachments/assets/49d2dbdc-b940-4aff-854a-9007957c2950)

#### Graph of mass versus radius in dimensionless units.
![image](https://github.com/user-attachments/assets/6f4ba791-f6cb-4fc3-95fb-44244c10bdc1)

#### Graph of Pressure versus radius in dimensionless units.
![image](https://github.com/user-attachments/assets/ce32ab37-0fd2-4409-b394-db81045da9a3)

#### Mass & Radius versus Energy Density (TOV)
![image](https://github.com/user-attachments/assets/a4c94a0f-328c-4059-8b6f-87f64327548b)

