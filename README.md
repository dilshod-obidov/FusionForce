# FusionForce
Project for Vertically Intagrated Project (VIP) 1

## Team Members:
- Dilshod Obidov (12225243) (Team Leader)
- WooSeok Kang (12213968)
- Nilufar Kurbonova (12225241)
- 

---
## Air-purifier Robot with Turtlebot3

---

1. Initialize the SDS011 sensor.
2. Read fine dust concentration data from the SDS011 sensor using PySerial.

3. Determine which room has the highest fine dust concentration:
   3.1. Compare fine dust concentration data for each room.
   3.2. Set the room with the highest concentration as the priority room.

4. Use ROS to communicate with the air-purifying robot.
5. Send the priority room information to the robot.

6. The air-purifying robot moves to the prioritized room:
   6.1. Use motor control and navigation algorithms to reach the room.
   6.2. Implement obstacle avoidance if necessary.

7. The robot initiates air purification in the priority room:
   7.1. Activate the air purification system.
   7.2. Monitor the fine dust concentration during the purification process.
   7.3. Continue purification until the concentration reaches an acceptable level.

8. Meanwhile, the sensor continues to detect the CO2 ratio:
   8.1. Read CO2 data from the sensor using PySerial.
   8.2. Compare the CO2 ratio to recommended standards.

9. If the CO2 ratio exceeds the recommended standard:
   9.1. ROS suggests ventilation as a remedy.
   9.2. The robot can initiate ventilation by opening windows or using a ventilation system.

10. Repeat the monitoring and purification process:
    10.1. Continue to monitor fine dust and CO2 levels.
    10.2. Update the priority room as needed based on changing conditions.

11. End of the process loop.
