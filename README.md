# Remote-Controlled Arduino Robot Arm

This project is based around a maker-buying robot arm which has an Arduino uno connected to its servo motors. This Arduino uno is connected to another one via the I2C protocol.
The controller and robot arm are currently very close to each other, but the wires can be replaced with longer ones, making it remote-controlled.
# Master:

This Arduino has two joysticks connected to it, which it checks the position of. It then sends the raw values to the slave.

# Slave:
This Arduino is connected to the servos of the robot arm and receives the values from the master Arduino. It then maps these values to more appropriate variables and sends them to the servo motors. I have programmed this Arduino to store the values of the servos locally and then move the servos accordingly. It's kind of hard to explain, but this is the principle used in all other machinery. Basically, the arm doesn't return to its original position when you release the joysticks. This and the i2c was by far the hardest part.

# Future Plans:
I plan to replace the Arduino Unos with ESP32s, which will allow me to make it wireless and use the wired I2C as a backup. This is a very big upgrade, but I think I can pull it off with just the right amount of time.

# Links:
Video: https://cloud-ih66h08m0-hack-club-bot.vercel.app/0robot-arm-video.mp4
Picture: https://cloud-gqmhao9w4-hack-club-bot.vercel.app/0robot-arm-picture.jpg

/ Hilding
