# parabola-plot
import numpy as np
import matplotlib.pyplot as plt

def plot_parabola(a=1, b=0, c=0):
    x = np.linspace(-10, 10, 400)  # Define x-axis range
    y = a * x**2 + b * x + c  # Parabola equation
    
    plt.figure(figsize=(8, 6))
    plt.plot(x, y, label=f'Parabola: {a}x² + {b}x + {c}', color='blue')
    plt.axhline(0, color='black', linewidth=0.5)
    plt.axvline(0, color='black', linewidth=0.5)
    plt.grid(True, linestyle='--', linewidth=0.5)
    plt.legend()
    plt.title("Parabola Graph")
    plt.xlabel("x-axis")
    plt.ylabel("y-axis")
    plt.show()

# Example usage
plot_parabola(a=1, b=2, c=-3)
wer
