# XenialDSR Program

## Overview

The XenialDSR program is designed to preprocess and organize financial data from a journal. It specifically handles the extraction of relevant information, grouping, and formatting for further analysis.

## Table of Contents

- [Features](#features)
- [Setup](#setup)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Features

1. **preProcess Method:**
   - Removes specified rows from the input data.
   - Groups rows by their column 0 and column 1 values.
   - Combines values in column 3 and adds values in column 4 if present.
   - Rounds values to 2 decimal places using `BigDecimal`.
   - Inserts combined rows back into the original format.

2. **finalProcess Method:**
   - Sorts the processed data by the `REFERENCE_NO`.
   - Attaches rows with "Total Tax," "Coupons," and "Delivery and Tips" after the last matching `REFERENCE_NO`.
   - Updates `lineNo` based on the `REFERENCE_NO`.

3. **processedDataArray:**
    -

## Setup

1. **Requirements:**
   - Java Development Kit (JDK) version 8 or later.

2. **Clone the Repository:**
   ```bash
   git clone https://github.com/amartinezjr7/xenialdsr.git
