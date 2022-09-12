# Solution to Case Interview

* Design and present the solution the way you usually do.

* Please make and state assumption (if any)

* Feel free to ask the question to get the neccessary information needed to complete the task.


## Case 1: Manage multiple site

For site of fast retail, there are event that marketing department want to spin up some quick temporary site for example for 9.9, 10.10, 11.11 campaign, special collection for specific targeted customers. On this page will have the list and price. However since this is static site, there will be an event of mismatch information for example, price.

Pain point: data mismatch for example price

Existing component: main site, api and databse

Task: Please provide solution to this case to solve the data mismatch issues


## Case 2: Race condition

Existing component: Core booking engine

Channel: Box office, Website, Mobile application

Process:
1. Pick the seat
2. Proceed with the checkout

Task: Please design the 2-3 solution and give a pros and cons comparison among those solution.

## Case 3: Data integrity

Existing Component: Source system export CSV data to the storage. We are building system to bring in this data on the daily basis e.g., every day 9 o'clock.

Process:
1. Source system export all information on the source table as CSV.
2. Our system bring in the data
3. Our system expose this data as an API

Task: Please design the solution to ensure data correctness and integrity in a timely manner.


## Case 3: Authentication

Existing material: User list in the CSV file.

Task: Please suggest the way to authentitcate agianst this list of the user.
