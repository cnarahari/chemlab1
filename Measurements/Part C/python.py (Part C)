import matplotlib.pyplot as plt
import numpy as np

# Experimental data
measurements = [1, 2, 3, 4]
densities = [9.7, 9.7, 9.7, 9.7]

# Calculate average density
average_density = np.mean(densities)

# Create bar graph
plt.bar(
    measurements,
    densities,
    color="skyblue",
    edgecolor="black"
)

# Add average density line
plt.axhline(
    y=average_density,
    color="red",
    linestyle="--",
    linewidth=2,
    label=f"Average Density ({average_density:.1f} g/cm³)"
)

# Labels and title
plt.xlabel("Measurement")
plt.ylabel("Density (g/cm³)")
plt.title("Density Measurements of a Penny")

# Make measurement numbers appear on x-axis
plt.xticks(measurements)

# Set y-axis range
plt.ylim(0, 11)

# Add legend
plt.legend()

# Improve layout
plt.tight_layout()

# Display graph
plt.show()
