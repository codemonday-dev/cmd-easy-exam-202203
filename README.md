# CODEMONDAY-technical-assignment-202203
Mini exam for CODEMONDAY's developer candidate of 2022

## Objective

**Create an API to handle the request which solve the problem as follows.**

Given: the shopping cart data of many items inside. \
Find: Total price amount in each category.
> The amount will be calculated by `unit_price x quantity`  
> To simplify the problem, there will be only three categories:  
> 1. sport
> 2. beverage
> 3. other (anything not in no. 1, 2)

## Sample input
Request JSON data to the server running on port 8080
```
POST http://localhost:8080/checkout

[
    {
        "item": "Nike Air Zoom",
        "category": "sport",
        "unit_price": 3000,
        "quantity": 1
    },
    {
        "item": "Protein Bar Herbalife Deluxe",
        "category": "sport",
        "unit_price": 50,
        "quantity": 10
    },
    {
        "item": "Starbucks Voucher",
        "category": "beverage",
        "unit_price": 500,
        "quantity": 1
    },
    {
        "item": "coffee",
        "category": "beverage",
        "unit_price": 20,
        "quantity": 10
    },
    {
        "item": "iPhone 13",
        "category": "electronic",
        "unit_price": 40000,
        "quantity": 1
    }ม
    {
        "item": "Cleaning alcohol",
        "category": "household",
        "unit_price": 5000,
        "quantity": 1
    }
]
```
---

## Sample output result
Expect the summary of ONLY
1. sport
2. beverage
3. other (anything not in "sport" and "beverage" categories)

So the response JSON data of the above example is:
```
{
  "result": {
      "sport": 3500,
      "beverage": 700,
      "other": 45000
  }
}
```
