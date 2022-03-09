# cmd-easy-exam-202203
Mini easy exam for candidate in 2022 March

# Sample input result
Request JSON to the server running on port 8080
```
POST localhost:8080/checkout
[
    {
        "item": "nike air zoom",
        "category": "sport",
        "unit_price": 3590,
        "quantity": 1
    },
    {
        "item": "protein bar",
        "category": "sport",
        "unit_price": 15.50,
        "quantity": 10
    },
    {
        "item": "Starbuck voucher",
        "category": "beverage",
        "unit_price": 200,
        "quantity": 1
    },
    {
        "item": "low-fat milk",
        "category": "beverage",
        "unit_price": 12.50,
        "quantity": 20
    },
    {
        "item": "iphone 13",
        "category": "electronic",
        "unit_price": 45000,
        "quantity": 1
    },
]
```

## Sample output result
Expect the summary of ONLY
1. sport
2. beverage
3. other (anything not sport and beverage)

```
{
    "controller": "checkout",
    "result": {
        "sport": 3745,
        "beverage": 450,
        "other": 45000
    }
}
```
