# Information about this Code_school_project
# NXT-MAP-Robot

This is the code for an NXT robot

it is the result of a school project where a process is to be automated.

This is one robot of three which make up a whole in the system. 
The project is called SCM-System and each letter stands for a task in the system.

The “S” stands for search robot, which searches for 4 found objects in an area and notes the position in the x and y directions and then sends this to the other two robots, which then collect the object and mark the position of the find on a map.

The “C” stands for collect robot, which collects the objects that have been found and takes them to a storage position. It then waits for the next coordinates, which it receives from the search robot.

The “M” stands for map robot, which draws a map (coordinate system with x-axis and y-axis as well as axis labeling) in a previously defined size and draws the position of the found object after receiving the coordinates.

The system works as follows:


- The robots were initially connected to each other via bluetooth
- The search robot then had to be calibrated, which was done using a compass, so that it knew where it was in order to send the exact coordinates to the remaining robots.
- Meanwhile, the map robot was started, which meant that it began to draw the map, as this took 3:16 minutes.
- the collecting robot has nothing to do during this time.
- while the search robot was searching for objects, the map robot was drawing the map and the collect robot was waiting for its turn.
- when the search robot found an object, it stopped and sent the x-coordinate and y-coordinate data to the collection robot first, and after sending the individual coordinates, waited for a confirmation of receipt so that the data actually arrived. When the collection robot received the data, it drove off while the data was sent to the map robot, which started drawing according to the same principle after confirmation of receipt.
- The collecting robot only waited for the data from the search robot and then it drove to the position and picked up the object.
- After the collecting robot received the data and confirmed receipt, it was the map robot's turn to receive the data, which it also confirmed and then started to draw the location.
 
