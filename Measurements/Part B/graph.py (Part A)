import matplotlib.pyplot as plt
import numpy as np

# Experimental data
measurements = [1, 2, 3, 4, 5]
densities = [0.876, 0.926, 0.968, 0.987, 0.973]

# Calculate average density and sample standard deviation
average_density = np.mean(densities)
standard_deviation = np.std(densities, ddof=1)

# True density of water
true_density = 0.99777

# Create bar graph with error bars
plt.bar(
    measurements,
    densities,
    yerr=standard_deviation,
    capsize=5,
    color="skyblue",
    edgecolor="black",
    error_kw={"ecolor": "black", "elinewidth": 1.5}
)

# Add average density line
plt.axhline(
    y=average_density,
    color="red",
    linestyle="--",
    linewidth=2,
    label=f"Average Density ({average_density:.3f} g/mL)"
)

# Add true density line
plt.axhline(
    y=true_density,
    color="green",
    linestyle="-",
    linewidth=2,
    label=f"True Density ({true_density:.5f} g/mL)"
)

# Labels and title
plt.xlabel("Measurement")
plt.ylabel("Density (g/mL)")
plt.title("Density of Water Measured Using a 100 mL Graduated Cylinder")

# Make measurement numbers appear on x-axis
plt.xticks(measurements)

# Set y-axis range
plt.ylim(0.80, 1.06)

# Add legend
plt.legend()

# Improve layout
plt.tight_layout()

# Display graph
plt.show()
