# Question 2: PSO and Differential Evolution

This question solves the Rosenbrock and Griewank equations using:

- Particle Swarm Optimization (PSO)
- Differential Evolution (DE)

Both implementations support multiple random seeds, report the best fitness
for each seed, calculate the mean and sample standard deviation of the final
fitness values, and store generation-level data for a convergence plot.

## Configuration

In either notebook, update these variables to change the experiment:

- `EVALUATION_FUNC_NAME` selects `evaluation_rosenbrock` or
  `evaluation_griewank`.
- `NUM_DECISION_VARIABLES` sets the number of decision variables.

The Differential Evolution notebook also exposes:

- `DE_SCALE_FACTOR` for the mutation scale factor.
- `DE_CROSSOVER_RATE` for the binomial crossover rate.

## Notebooks

- [`src/pso_implementation.ipynb`](src/pso_implementation.ipynb) —
  Particle Swarm Optimization.
- [`src/differential_evolution_impl.ipynb`](src/differential_evolution_impl.ipynb) —
  Differential Evolution.

## Results

The following summary shows the mean and standard deviation of the final
fitness values across the configured seeds for both algorithms:

![PSO and Differential Evolution fitness summary](results-q2-summary.png)

## Requirements

Install the required packages with:

```bash
python -m pip install deap numpy matplotlib jupyter
```

## Running the Notebooks

From the repository root, start Jupyter:

```bash
jupyter notebook
```

Open either notebook and run its cells from top to bottom.
