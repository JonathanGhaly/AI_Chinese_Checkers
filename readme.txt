////////////////////////////////
Programming Language: Python 3.9
////////////////////////////////
Running Steps:
    1. Run main_menu.py
    2. Click on any red piece (human is the red player on top) and move it to the available place
///////////////////////////////
Heuristic Description:
    The heuristic is composed of 3 steps:
        1. Calculate xend and yend for the board.
            - xend is calculated based on the position of the last marble in the enemy's base
            - yend for a certain player is calculated by looping through all spaces in the matrix that are not
            occupied by this player, where empty (white) spaces are assigned much greater value than enemy covered spaces.
        2. Calculate the avg distance for every marble of a certain player based on each individual marble's location
        3. Calculate the heuristic value by computing: red_heuristic - green heuristic
            - green player is considered as winning if the value of red_heuristic - green heuristic keeps increasing
            and vice versa for the red player
///////////////////////////////
Team Info:
Name                ID              Emails
Jonathan Saad       20190158        jghaly00@gmail.com
David Ayman         20190196        davidmorcos3720@gmail.com
Shehab Gad          20190818        shehabgad2@gmail.com
Peter Essam         20190141        pessam33@gmail.com