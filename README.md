# ninja-3

# Ninja-game

For our jQuery practice, you're going to make a game. We will call this game, Ninja Gold. jQuery does both DOM manipulation (HTML, CSS) and data manipulation. We will practice both. The Ninja moving around will be the DOM part and the log will be the data manipulation part.
Our main character is a ninja in search for gold. 

## Objective
He can find gold in 4 different places: the cave, the house, the goldmine and at the casino. 

In 20 trys, the ninja should reach 250 gold. If the ninja doesn't fail, restart the game.

## Probability ## 

•	cave 100% + 5 gold
•	house 80% + 10 gold
•	goldmine 80% + 1 - 25 gold (random)
•	casino 50% (+ OR -) 40 - 50 gold (random)

## Features ##
•	Counter for number of attemps
•	Counter for total gold. Make it red if he loses money, black if 0 gain or loss and green if he gains money
•	A log of the event. If the ninja loses money, make the log text color red and green if he gains money.
•	Reset button (gold 0 and trys 20)
•	Different locations with buttons (no need for actual pictures of the location)
•	A ninja sprite that moves around the different locations. (when you click goldmine, he will move to goldmine. When you click casino he will move to the casino)

## Other Notes ##
For the log, use an array of events (json object contains data like the time, location and amount)
```
{
  time: 'some date string',
  amount: -40
}

One possible data structure might be 
{   
    total: 0,
    attempts:20,
    events: [],
}

```

Use the same events array for getting the total score. Or you can store it inside the object as total.  

## Log ###
- Use bootstrap tabs to sort the different logs. All, Losses, Gains.
- Create separate arrays for logging negative and positive events. 
- Also put the total gains and total losses.
- Learn to use Array.filter or Array.reduce Array.map functions. You can use jQuery equivalents $.each and $.map

## Bonus ##
- Persist the data (score and log) even with a browser refresh.
- Deploy it using surge.sh


