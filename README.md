# CODEMONDAY-live-code-interview (API based)
Live-code interview question for CODEMONDAY's software developer (year 2022).

## Question 1
### Objective
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

```
{
  "result": {
      "sport": 3500,
      "beverage": 1500,
      "other": 45000
  }
}
```

---
---
---
---
---
---
---
---
---

# CODEMONDAY-live-code-interview (JavaScript based)
Live-code interview questions for CODEMONDAY's software developer (year 2022).

## Question 2
Given: Array of number `[1, 2, 3, 4, 5, 6, 7]`.

Find: Expect array of number which elements are calculated from the even number of input array times two (เอาค่าใน Array Input ที่เป็นเลขคู่ มาคูณด้วย 2)

#### Input
```js
[1, 2, 3, 4, 5, 6, 7]
```

#### Expected Output
```js
[4, 8, 12]
```

---

## Question 3
Given: Collection of users (array of user object).

Find: 
> (a) Find the name of the user who has maximum age.
> 
> (b) Create function to get age by name, e.g., `getAgeByName('Boat')` or `getAgeByName('boat')` will get result `26`
> 
> (c) Transform array and grouping into `[{ 25: ['Win', 'Ton'], 33: ['Jeff'], 26: ['Boat']}]`

#### Input
```js
[
  {
    name: 'Win',
    age: 25
  },
  {
    name: 'Ton',
    age: 25
  },
  {
    name: 'Jeff',
    age: 33
  },
  {
    name: 'Boat',
    age: 26
  }
]
```

#### Expected Output
```
(a) "Jeff" (name of the user who has maximum age)
(b) getAgeByName('boat') will get 26.
(c) [{ 25: ['Win', 'Ton'], 33: ['Jeff'], 26: ['Boat']}]
```

----

## Question 4
Given: UI image. \
![Image of React Counter](https://github.com/codemonday-dev/cmd-easy-exam-202203/blob/main/counter-plain.png)

Find: Make UI for the counter gadget with interaction as in the given image

> **Acceptance Criteria**:
> 1. Initial state should display 0
> 2. When click '+', increment the displayed number by 1
> 3. When click '-', decrement the displayed number by 1


----

## Question 5

Given: Any odd number, ex. `1`, `7`, `35`, `99`.
Find: Create function to print (console) the Cross sign made from `*` and space ` ` character print to console.

#### Expected Output
Input: `num = 3`
```
* *
 *
* *
```

Input: `num = 5`
```
*   *
 * *
  *
 * *
*   *
```


Input:`num = 9`
```
*       *
 *     * 
  *   *  
   * *   
    *    
   * *   
  *   *  
 *     * 
*       *
```
