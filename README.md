# CSCTFShareWebPage
Webpage to calculate percentage shares

Objective - Learning how to use jQuery and JavaScript.

Formulas

Initial share - share value before bonus  
Final share - share value after adding the bonus rewards

USER_POINTS = How many points the user recieved in CSCTF  
TOTAL_POINTS = Total points of all players in a guild.  
REWARD_POINTS = Amount of CPs (or any general reward points)  
BONUS_REWARDS = The total amount of extra rewards given to certain players (Can be in CPs or any reward point in general) 
USER_BONUS = THe amount of extra reward the user recieves. 

Share (Initial Share) = (USER_POINTS / TOTAL_POINTS) * REWARD_POINTS  
Share (Final) = (USER_POINTS / TOTAL_POINTS) * (REWARD_POINTS - BONUS_REWARDS) + USER_BONUS

To calculate the percentage of work the user has done, we divide the users points and the total points of all participants, then multiply it by the reward points.
At some point, maybe a leader may decide they want to give bonus rewards to certain players to balance things out. So the final share handles that problem
The total reward will be subtracted by the total amount of bonus rewards given out. Then give out the percentage of shares based on the new available reward amount along with the bonus points.

# CSCTF Points
Calculate CSCTF Points. This is under the assumption that you're in x2 base the full hour

Formula

USER_CSCTF_POINTS = Kills + shackles + unshackles + revive + flags_captured + flags_delivered   
KILLS_PER_POINTS = 1  
SHACKLE_PER_POINTS = 1  
UNSHACKLE_PER_POINTS = 1  
REV_PER_POINTS = 2  
FLAGS_CAP_PER_POINTS = 3  
FLAGS_DELIVER_PER_POINTS = 30 
