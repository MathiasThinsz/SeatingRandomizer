# SeatingRandomizer

Please help me out with creating a table seating randomizer!

I would like to have an application helping me do the table seating at larger parties! I'd like an application randomizing the seats and here is the feature requests for version 1.0:

# Specification
## Input variables:
- List of tables with seats. Eg if there are 6 tables, 2 with 6 seats and 4 with 8 seats this list would be: tables[6,6,8,8,8,8]
- List of guests. The guests can be couples or singles, this example shows the first 12 guests: guests["Anna,Johan","Niklas","Lisa,Noah","Eva,Erik","Malin,Lars P.","Annika","Linda,Elin"]
- Boolean allowing couples to be split or not: `allowSplittedCouples` true/false

## Functionality
- there are three seatings: entrée, main course, dessert. 
- the app should present three randomly created seatings, one for each seating (entrée, main course, dessert)
- the app should avoid seating guests that previously have been seated at the same table at a previous seating. This is the main purpose of the app. If an app user has many guests and few tables this will be harder to accomplish, but the user must understand that smaller tables are needed in that case.
- `allowSplittedCouples` is false by default and if `allowSplittedCouples` is false then couples must be seated at the same table for all three seatings.

