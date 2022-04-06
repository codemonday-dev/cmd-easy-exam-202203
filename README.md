# CODEMONDAY-technical-assignment-2022
Exam for CODEMONDAY's software developer candidate (2022)

## Objective

**Create an API to handle the request which solve the problem as follows.**

Given: the shopping cart data of many items inside.

Find: Total price amount in each category.
> The amount will be calculated by `unit_price x quantity`  
> To simplify the problem, there will be only three categories:  
> 1. sport
> 2. beverage
> 3. other (anything not in "sport" and "beverage" categories)

#### Input
Request JSON data to the server running on port 8080

POST http://localhost:8080/checkout

Request Body
```

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
        "item": "Starbucks Coffee",
        "category": "beverage",
        "unit_price": 500,
        "quantity": 3
    },
    {
        "item": "iPhone 13",
        "category": "electronic",
        "unit_price": 40000,
        "quantity": 1
    },
    {
        "item": "Cleaning alcohol",
        "category": "household",
        "unit_price": 5000,
        "quantity": 1
    }
]
```

---

#### Expected Output
Expect the summary of ONLY

```
{
  "result": {
      "sport": 3500,
      "beverage": 1500,
      "other": 45000
  }
}
```
