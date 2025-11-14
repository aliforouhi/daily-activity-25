# daily_update.p
import datetime
import random

print("Daily GitHub activity - Day 25")

today = datetime.date.today()

# Generate a dictionary of random values
data = {f"item_{i}": random.randint(1, 500) for i in range(1, 6)}

highest_key = max(data, key=data.get)
lowest_key = min(data, key=data.get)

print(f"Today's date: {today}")
print(f"Generated dictionary: {data}")
print(f"Highest value: {highest_key} -> {data[highest_key]}")
print(f"Lowest value: {lowest_key} -> {data[lowest_key]}")
