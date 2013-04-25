# Brainstorming:

The game will consist of the following components: 

## A Technology Tree, which contains:

- Telescopes
    - Cost: x
    - Allows: a larger radius of revealed area around the planet
    - Upgrades: increase radius
- Unmanned Missions
    - Cost: x
    - Allows: uni-directional exploratory missions
    - Upgrades: increase distance before contact is lost
- Mining Operations
    - Cost: x
    - Allows: extracting resources from planetary bodies
    - Upgrades: increase efficiency of mining, allows mining of more valuable resources
- Transport Missions
    - Cost: x
    - Allows: sending resources between colonies/planets
    - Upgrades: transport a higher quantity of resources, with a lower chance of failure (and defense against pirates)
- Manned Missions
    - Cost: x
    - Allows: researching colonizing
    - Upgrades: increase chance of mission succeeding
- Colonizing
    - Cost: x
    - Allows: building additional colonies
    - Upgrades: increase chance of mission succeeding

## Colonies, which have:

- Actions (the ability to launch missions, based on researched technology)
- Inventory (a collection of unsold resources)

## Resources (a collection of resource objects, which each have):

- Value (a range that determines the possible selling price on various colonies)
- Scarcity (a range that determines the likelihood of finding this resource on any given planet)
- Demand (a range that determines the likelihood of colonies being willing to buy this resource)

## Space, which has:

- A grid (to handle the coordinates of various planetary bodies)
- Planetary bodies, which include
    - Asteroids, which have
        - Resources (80%)
    - Small Planets, which have
        - Moons (75% 0, 25% 1)
        - Resources (40%)
    - Medium Planets, which have
        - Moons (25% 0, 50% 1, 25% 2)
        - Resources (100%)
        - Potential for colonization
        - Existing alien colonies, willing to trade
    - Large Planets
        - Moons (20% 2, 20% 3, ... 20% 6)
        - Resources (0% -- all large planets are gassy)
    - Moons
        - Resources (20%)

## A User, who has

- Currency (which can be spent on research or missions)
- Researched Technology (a subset of the full tech tree)
- A map (a representation of "Space" that only reveals discovered coordinates)
