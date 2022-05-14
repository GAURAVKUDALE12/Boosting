# Boosting
XGM &amp; LGBM


## Problem Statement: 

**Tennis Australia open is trying to better automate how tennis points get categorized into three outcomes – winners, forced errors and unforced errors.**

## Dataset Description:

The dataset includes point outcomes of rallies only (where the number of shots hit exceeds two, which represents the serve and return). All points were played at a past Australian Open.


### Target

#### Outcome variable - classes
* Winner – the point winning player hits a shot that is not touched by the opponent
* Forced error – the point winning player hits a shot that causes the opponent to not be able to return it, i.e. a good shot that is hard to handle
* Unforced error – the player attempting to return the ball makes an error on an otherwise normal looking rally shot

# Atribute description

| Variable | Description| Value Range |
| :- | -: | :-: |
rally | The number of shots in the point counting serves and point-ending shot | An integer from 1, 2, 3...
| serve | A number indicating whether the point was played on a first or second serve.  | 1 = First, 2 = Second
| hitpoint | Shot category for point-ending shot | F = Forehand, B = Backhand, V = Volley, U = Unknown
| speed | Speed of point-ending shot | Continuous (m/s)
| net.clearance | Distance above the net as point-ending shot passed the net | Continuous (cm) distance above net. Can be negative if shot did not pass above the net.
| distance.from.sideline | Lateral distance of the point-ending shot bounce from the nearest singles sideline. | Perpendicular distance in meters (always positive even if out)
| depth | Distance of the point-ending shot bounce from the baseline | Perpendicular distance in meters
(always positive even if out)
| outside.sideline | Logical indicator of whether point-ending shot landed outside of the in-play singles sideline | TRUE, FALSE
| outside.baseline | Logical indicator of whether point-ending shot landed beyond the in-play baseline | TRUE, FALSE
| player.distance.travelled | Distance player who made the point-ending shot travelled between the impact of the penultimate shot and the impact of the point-ending shot | Euclidean distance in meters
| player.impact.depth | Distance of player who made point-ending shot from the net at the time the point-ending shot was made | Perpendicular distance along the length of court from net in meters
| player.impact.distance.from.center | Distance of player who made point-ending shot from the center line at the time the point-ending shot was made | Perpendicular distance from the center line in meters
| player.depth | Distance of player who made point-ending shot from the net at the time the penultimate shot was made | Perpendicular distance along the length of court from net in meters
| player.distance.from.center | Distance of player who made point-ending shot from the center line at the time the penultimate shot was made | Perpendicular distance from the center line in meters
| opponent.depth | Distance of opponent from the net at the time the at the time the penultimate shot was made | Perpendicular distance along the length of court from net in meters
| opponent.distance.from.center | Distance of opponent from the center line at the time the penultimate shot was made | Perpendicular distance from the center line in meters
| same.side | Logical indicator if both player and opponent were positioned on the same side of the center line (ad or deuce court) at the time the penultimate shot was made | TRUE, FALSE
| previous.speed | Speed of penultimate shot | Continuous (m/s)
| previous.net.clearance | Distance above the net as penultimate shot passed the net | Continuous (cm) distance above net. Can be negative if shot did not pass above the net.
| previous.distance.from.sideline | Lateral distance of the penultimate  shot bounce from the nearest singles sideline. | Perpendicular distance in meters (always positive even if out)
| previous.depth | Distance of the penultimate shot bounce from the baseline | Perpendicular distance in meters
(always positive even if out)
| previous.hitpoint | Shot category for penultimate shot | F = Forehand, B = Backhand, V = Volley, U = Unknown
| previous.time.to.net | Time for penultimate shot to be hit and pass the net | Continuous number in seconds
| server.is.impact.player | Logical if player who made point-ending shot was the server of the point | TRUE, FALSE
| outcome | Target variable, character with three categories indicating the type of shot that ended the point  | W (Winner), FE (Forced Error), UE (Unforced Error)
| id | A 10-character unique identifier for the point | Character
