# Parking Fare Calculation Program

This program calculates the daily parking fare for customers who park their vehicles in a parking lot based on the type of vehicle, parking duration, and discount rate. It includes various features such as handling different vehicle types, discount rates, and more.

## Problem Overview

The program takes the following inputs:
- **Vehicle Type**: A string indicating the type of vehicle (Car, Bus, Truck).
- **Number of Hours Parked**: An integer representing the number of hours the vehicle was parked.
- **Number of Minutes Parked**: An integer showing the number of minutes the vehicle was parked (e.g., 2 hours 40 minutes).
- **Discount Type**: A string that represents the type of customer (D for Daily customer, W for Weekly customer, I for Irregular customer).

### Parking Rates

The rates are as follows:

| Vehicle Type | First Rate                        | Second Rate                      |
|--------------|-----------------------------------|-----------------------------------|
| **Car**      | $5.00 per hour for the first 3 hours | $2.00 per hour after the first 3 hours |
| **Truck**    | $6.00 per hour for the first 2 hours | $2.50 per hour after the first 2 hours |
| **Bus**      | $12.00 per hour for the first hour | $4.25 per hour after the first hour |

### Discount Rates

Discounts are applied based on customer type:
- **Daily**: 5% discount
- **Weekly**: 3% discount
- **Irregular**: 0% discount

### Parking Duration Rules
- If the vehicle is parked for 1 hour 1 minute to 2 hours, the user is charged for 2 hours.  Any minute over an hour adds an additional hour to the charge.

## Features
- **Clear Instructions to User**:  Be sure to instruct the user as to what they are entering.
- **Formatted Output**: The output will be displayed in a monetary format of `$##.##`.  Display all output clearly.
- **Methods**: Methods can be utilized but are not required.
- **Documentation**:  Be sure to include header documentation and code documentation.

## Test Data

Here are some test cases for the program:

| Vehicle | Time in Lot             | Discount Type | Calculated Fare |
|---------|-------------------------|---------------|-----------------|
| Car     | 2 hours 20 minutes      | D             | Fare = $14.25   |
| Truck   | 7 hours 59 minutes      | W             | Fare = $26.19   |
| Bus     | 5 hours 12 minutes      | I             | Fare = $33.25   |
| Car     | 7 hours 0 minutes       | W             | Fare = $22.31   |
| Bus     | 0 hours 40 minutes      | D             | Fare = $11.40   |
| Truck   | 17 hours 1 minute       | I             | Fare = $52.00   |


## Bonus Features
1. **Error Message for Invalid Inputs**: The program should display an error if the user enters an invalid amount.
2. **Case-Insensitive Input**: The program should work regardless of the case (e.g., CAR, car, or Car).
3. **Entry and Exit Time Calculation**: Calculate the parking duration using entry and exit times in military format, handling any discrepancies between them.

