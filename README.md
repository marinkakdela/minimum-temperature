# minimum-temperature
def calculate_pressure(force, area):
    """Calculate pressure given force and area."""
    if area <= 0:
        return "Area must be greater than zero!"
    return force / area

def find_min_temperature(temperatures, unit="C"):
    """Find the minimum temperature from a list in Celsius or Kelvin."""
    if not temperatures:
        return "Temperature list is empty!"
    min_temp = min(temperatures)
    if unit == "K":
        return min_temp + 273.15  # Convert Celsius to Kelvin
    return min_temp

# Example usage
force = 500  # Newtons
area = 2  # Square meters
pressure = calculate_pressure(force, area)
print(f"Pressure: {pressure} Pascals (N/m²)")

temperatures = [-10, -20, 5, 0, -15, -30]
min_temp_c = find_min_temperature(temperatures, "C")
min_temp_k = find_min_temperature(temperatures, "K")
print(f"Minimum Temperature: {min_temp_c} °C")
print(f"Minimum Temperature: {min_temp_k} K")
12sdeq
