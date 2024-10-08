import numpy as np

# Generate synthetic Doppler shift data (in Hz)
doppler_data = np.array([1.2, 2.1, 1.5, 2.5, 3.0])

# Constants
frequency_emitted = 2e6  # 2 MHz ultrasound
speed_of_sound = 1540  # speed of sound in soft tissue, m/s

# Calculate blood flow velocity (in m/s)
velocity = (doppler_data * speed_of_sound) / (2 * frequency_emitted)

print("Blood flow velocities (m/s):", velocity)
