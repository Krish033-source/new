# Python Sum Calculator
## Introduction
This is a simple Python program designed to calculate the sum of a list of numbers.

## Features
* Calculate the sum of a list of numbers
* Handle empty lists
* Handle non-numeric input

## Requirements
* Python 3.x

## Installation
1. Clone the repository: `git clone https://github.com/your-username/python-sum-calculator.git`
2. Navigate to the project directory: `cd python-sum-calculator`
3. Install dependencies: `pip install -r requirements.txt`

## Usage
1. Run the program: `python sum_calculator.py`
2. Enter a list of numbers separated by commas: `1, 2, 3, 4, 5`
3. The program will output the sum: `15`

## Code
```python
def calculate_sum(numbers):
    try:
        return sum(float(num) for num in numbers)
    except ValueError:
        return "Invalid input: please enter a list of numbers"

def main():
    user_input = input("Enter a list of numbers separated by commas: ")
    numbers = [num.strip() for num in user_input.split(',')]
    result = calculate_sum(numbers)
    print(result)

if __name__ == "__main__":
    main()
```

## Example Use Cases
* Calculating the sum of a list of exam scores
* Calculating the sum of a list of numbers in a mathematical expression

## Contributing
Pull requests are welcome! To contribute, please fork the repository and submit a pull request with your changes. 

## License
MIT License

## Contact
For questions or feedback, please contact [Your Email](mailto:your-email@example.com)