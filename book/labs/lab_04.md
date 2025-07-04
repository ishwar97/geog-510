---
jupytext:
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.16.7
kernelspec:
  display_name: Python 3 (ipykernel)
  language: python
  name: python3
---

# Lab 4

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ishwar97/geog-510/blob/main/book/labs/lab_04.ipynb)

+++

## Exercise 1: Variable Assignment and Basic Operations

Create variables to store the following geospatial data:

- The latitude and longitude of New York City: 40.7128, -74.0060.
- The population of New York City: 8,336,817.
- The area of New York City in square kilometers: 783.8.

Perform the following tasks:

1. Calculate and print the population density of New York City (population per square kilometer).
2. Print the coordinates in the format "Latitude: [latitude], Longitude: [longitude]".

```{code-cell} ipython3

```

## Exercise 2: Working with Strings

Create a string variable to store the name of a city, such as "San Francisco". Perform the following operations:

1. Convert the string to lowercase and print the result.
2. Convert the string to uppercase and print the result.
3. Replace "San" with "Los" in the city name and print the new string.

```{code-cell} ipython3

```

## Exercise 3: Using Lists

Create a list of tuples, where each tuple contains the name of a city and its corresponding latitude and longitude:

- New York City: (40.7128, -74.0060)
- Los Angeles: (34.0522, -118.2437)
- Chicago: (41.8781, -87.6298)

Perform the following tasks:

1. Add a new city (e.g., Miami: (25.7617, -80.1918)) to the list.
2. Print the entire list of cities.
3. Slice the list to print only the first two cities.

```{code-cell} ipython3

```

## Exercise 4: Using Tuples

Create a tuple to store the coordinates (latitude, longitude) of the Eiffel Tower: (48.8584, 2.2945). Perform the following tasks:

1. Access and print the latitude and longitude values from the tuple.
2. Try to change the latitude value to 48.8585. What happens? Explain why.

```{code-cell} ipython3

```

## Exercise 5: Working with Sets

Create a set of countries you have visited, such as {"USA", "France", "Germany"}. Perform the following tasks:

1. Add a new country to the set.
2. Try to add the same country again. What happens?
3. Print the updated set.

```{code-cell} ipython3

```

## Exercise 6: Working with Dictionaries

Create a dictionary to store information about a specific geospatial feature, such as a river:

- Name: "Amazon River"
- Length: 6400 km
- Countries: ["Brazil", "Peru", "Colombia"]

Perform the following tasks:

1. Add a new key-value pair to the dictionary to store the river's average discharge (e.g., 209,000 m³/s).
2. Update the length of the river to 6992 km.
3. Print the dictionary.

```{code-cell} ipython3

```

## Exercise 7: Nested Data Structures

Create a dictionary to represent a city that contains the city's name, population, and coordinates (latitude, longitude):

- Name: "Tokyo"
- Population: 13,515,271
- Coordinates: (35.6895, 139.6917)

Perform the following tasks:

1. Access and print the population of the city.
2. Access and print the city's latitude.
3. Update the population to 14,000,000 and print the updated dictionary.

```{code-cell} ipython3

```

## Exercise 8: List Operations

Given the list of cities from Exercise 3, perform the following operations:

1. Sort the list of cities alphabetically by name.
2. Create a new list that contains only the city names.
3. Remove the last city from the original list and print the updated list.

```{code-cell} ipython3

```

## Exercise 9: Dictionary Operations

Using the dictionary from Exercise 6, perform the following tasks:

1. Check if the key "Length" exists in the dictionary.
2. Print all the keys in the dictionary.
3. Print all the values in the dictionary.

```{code-cell} ipython3

```

## Exercise 10: Practical Application

Imagine you have a list of tuples, each representing a location with its name, latitude, and longitude:

```{code-cell} ipython3
locations = [
    ("Mount Everest", 27.9881, 86.9250),
    ("K2", 35.8808, 76.5155),
    ("Kangchenjunga", 27.7025, 88.1475),
]
```

Perform the following tasks:

1. Create a new list that contains only the names of the locations.
2. Create a dictionary where the keys are location names and the values are tuples of their coordinates.
3. Print the latitude of "K2" using the dictionary.

```{code-cell} ipython3

```

## Exercise 11: Manipulating Geographic Location Strings

- Create a string that represents the name of a geographic feature (e.g., `"Amazon River"`).
- Convert the string to lowercase and then to uppercase.
- Concatenate the string with the name of the country (e.g., `"Brazil"`) to create a full location name.
- Repeat the string three times, separating each repetition with a dash (`-`).

```{code-cell} ipython3

```

## Exercise 12: Extracting and Formatting Coordinates

- Given a string with the format `"latitude, longitude"` (e.g., `"40.7128N, 74.0060W"`), extract the numeric values of latitude and longitude.
- Convert these values to floats and remove the directional indicators (`N`, `S`, `E`, `W`).
- Format the coordinates into a `POINT` WKT string (e.g., `"POINT(-74.0060 40.7128)"`).

```{code-cell} ipython3

```

## Exercise 13: Building Dynamic SQL Queries

- Given a table name and a condition, dynamically build an SQL query string.
- Example: If `table_name = "cities"` and `condition = "population > 1000000"`, the query should be `"SELECT * FROM cities WHERE population > 1000000;"`.
- Add additional conditions dynamically, like `AND` clauses.

```{code-cell} ipython3

```

## Exercise 14: String Normalization and Cleaning

- Given a list of city names with inconsistent formatting (e.g., `[" new york ", "Los ANGELES", "   CHICAGO"]`), normalize the names by:
  - Stripping any leading or trailing whitespace.
  - Converting them to title case (e.g., `"New York"`, `"Los Angeles"`, `"Chicago"`).
- Ensure that the output is a clean list of city names.

```{code-cell} ipython3

```

## Exercise 15: Parsing and Extracting Address Information

- Given a string in the format `"Street, City, Country"` (e.g., `"123 Main St, Springfield, USA"`), write a function that parses the string into a dictionary with keys `street`, `city`, and `country`.
- The function should return a dictionary like `{"street": "123 Main St", "city": "Springfield", "country": "USA"}`.

```{code-cell} ipython3

```

## Exercise 16: Using For Loops to Process Coordinate Lists

- Create a list of tuples representing coordinates (latitude, longitude).
- Write a `for` loop that prints each coordinate and indicates whether it is in the Northern or Southern Hemisphere based on the latitude.

```{code-cell} ipython3

```

## Exercise 17: While Loops for Iterative Processing

- Create a list of coordinates (latitude, longitude).
- Write a `while` loop that continues to print each coordinate until it encounters a coordinate with a negative latitude.
- Stop the loop once this condition is met.

```{code-cell} ipython3

```

## Exercise 18: Conditional Logic in Loops

- Create a list of coordinates and use a `for` loop to iterate over them.
- Use an `if-elif-else` statement inside the loop to classify each coordinate based on its longitude:
  - Print `"Eastern Hemisphere"` if the longitude is greater than 0.
  - Print `"Western Hemisphere"` if the longitude is less than 0.

```{code-cell} ipython3

```

## Exercise 19: Filtering Data with Combined Loops and Conditionals

- Given a list of coordinates, filter out and store only those located in the Southern Hemisphere (latitude < 0).
- Count the number of coordinates that meet this condition and print the result.

```{code-cell} ipython3

```

## Exercise 20: Generating and Analyzing Random Coordinates

- Write a program that generates random coordinates (latitude between [-90, 90] degrees and longitude between [-180, 180] degrees).
- Use a `while` loop to keep generating coordinates until a pair with both latitude and longitude greater than 50 is generated.
- Print each generated coordinate and the final coordinate that meets the condition.

```{code-cell} ipython3

```

## Submission Requirements

Complete the exercises above and and upload the notebook to your GitHub repository. Make sure the notebook has a Colab badge at the top so that it can be easily opened in Google Colab. Submit the URL of the notebook to Canvas.
