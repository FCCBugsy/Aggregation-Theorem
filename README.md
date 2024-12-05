# Aggregation Theorem (Subnets)

## Overview

The Aggregation Theorem provides a simple and intuitive formula for calculating the parent network mask when aggregating multiple subnets. This approach simplifies subnetting and supernetting tasks for network engineers and students.

**Formula**:
Parent Mask = Original Mask - log2(Number of Subnets)

This repository introduces the theorem, demonstrates its application, and provides practical examples to aid understanding.
## Applications

### Example 1: Aggregating 4 Subnets
- **Subnets**: `192.168.1.0/26`, `192.168.1.64/26`, `192.168.1.128/26`, `192.168.1.192/26`
- **Original Mask**: `/26`
- **Number of Subnets**: 4
- **Calculation**: Parent Mask = 26 - log2(4) = 26 - 2 = 24
- **Parent Network**: `192.168.1.0/24`

### Example 2: Aggregating 8 Subnets
- **Subnets**: `10.0.0.0/27` (and 7 others in the same range)
- **Original Mask**: `/27`
- **Number of Subnets**: 8
- **Calculation**: Parent Mask = 27 - log2(8) = 27 - 3 = 24
- **Parent Network**: `10.0.0.0/24`

## License
This project is released under the [MIT License](./license.txt). Feel free to use and adapt it, but please credit the author (Bugsy).

## Author
Created by **Bugsy**, published under a pseudonym for privacy reasons.


