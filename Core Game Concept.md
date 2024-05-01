**Core Game Concept**

- **Objective:** Transport all three missionaries and three cannibals from one bank of a river to the other.
- **Boat Capacity:** The boat can carry a maximum of two people.
- **Cannibal Constraint:** At no point can cannibals outnumber missionaries on either bank of the river, or else the missionaries will be in serious trouble!
- **Win Condition:** All missionaries and cannibals reach the opposite bank safely.
- **Loss Condition:** Cannibals outnumber missionaries on a bank.

**Notes: Data Structures**

- **Representing Game State:** We will use a dictionary.
    
    Python
    
    ```Python
    game_state = {
        "left_missionaries": 3,  
        "left_cannibals": 3,
        "right_missionaries": 0, 
        "right_cannibals": 0,
        "boat": "left"  # or "right"
    }
    ```
    

