# **Mean-Variance-Standard-Deviation-Calculator**
This is the boilerplate for the Mean-Variance-Standard Deviation Calculator project. Instructions for building your project can be found at https://www.freecodecamp.org/learn/data-analysis-with-python/data-analysis-with-python-projects/mean-variance-standard-deviation-calculator

## **Project Overview**

The ```calculate()``` function in ```mean_var_std.py``` takes a list of 9 digits and transforms them into a $3 \times 3$ NumPy array. It then calculates the following metrics:
* Mean
* Variance
* Standard Deviation
* Max / Min
* Sum

For each metric, the function provides values calculated across Axis 0 (columns), Axis 1 (rows), and the flattened matrix (all elements).

## **Features**
* Input Validation: Automatically checks if the input list contains exactly 9 elements.
* Error Handling: Raises a ValueError with a specific message if the input is invalid.
* Data Conversion: Ensures all NumPy outputs are converted back into standard Python lists for easier JSON compatibility or further processing.

## **Installation**

1. Clone the repository:

```Bash
   git clone https://github.com/your-username/mean-var-std-calculator.git

   cd mean-var-std-calculator
```

3. Install dependencies:

This project requires NumPy. Due to recent compatibility updates, it is recommended to use a version that matches your environment (see the Troubleshooting section if you encounter errors).

```Bash
pip install numpy
```

## **Usage**

Import the function into your Python script and pass a list of nine integers:
```Python
import mean_var_std
result = mean_var_std.calculate([0, 1, 2, 3, 4, 5, 6, 7, 8])
print(result)
```

## **Expected Output Format**:

```Python
{
  'mean': [[3.0, 4.0, 5.0], [1.0, 4.0, 7.0], 4.0],
  'variance': [[6.0, 6.0, 6.0], [0.66, 0.66, 0.66], 6.66],
  'standard deviation': [[2.44, 2.44, 2.44], [0.81, 0.81, 0.81], 2.58],
  'max': [[6, 7, 8], [2, 5, 8], 8],
  'min': [[0, 1, 2], [0, 3, 6], 0],
  'sum': [[9, 12, 15], [3, 12, 21], 36]
}
```

## **License**
This project is open-source and available under the MIT License.
