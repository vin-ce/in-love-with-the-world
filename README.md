# Simulation

Each cell contains an `awareness` amount. This is currently in 0.25 increments

`curDirectoin` is to maintain a direction that the cell move towards

`hasMoved` is to prevent the cell from moving again after it's cycled through it once

`cyclesAlive` helps track how long it should be alive for


## Step Grid

The position is stepped first. 

First it looks at what directions are available by checking the awareness value. It the available directions in an array

Then it figures out what the next direction should be. 

If there isn't a direction already available, then it chooses a random one from the `availableDirections` array. 

If there is, then it checks the 3 cells in its 'front', checks their availability, and either successfully assigns a new direction (with the forward direction weighted more), or randomly assigns a direction if none of the front directions are free.

## Step Attribute

Figures out and increments up the neighbours based on %. Greater percentage increases it by 1.




The attribute is then stepped (emotion)




cells 'die' in `modulateAwareness`. Values for each cell are thus reset there





## To Do
- consider visuals
- patterning at different scales
  - mind as agent vs thought cells as agent
- different movement patterns for the cell (e.g a cell moves in circles)
- narrative!


## 2021-07-06 (2021-07-05 in US time)
- different mind states are actually possible
  - you can have way higher than average baseline happiness state (Nick Cammarata)
  - what might an interesting mind state look like in this sim?
  - what's the 'takeaway'?
    - how to craft presentation & narrative to impress the idea of greater possibility space?


## 2021-07-19
- mind types:
  - rumminator
    - form 1: make obsessive on a single thought
      - not many thoughts, but the thoughts that do come up stay around forever
    - form 2: many low-med continually cycling
  - meditator
  - volatile
  - 'average'
  - good natured
    - 'never gets angry'
    - can have many 25% milling around