# weekly log
# week 6:
## Project Proposal
The group members intended to define a design direction, and we each conceived two options for discussion. After the group's exchange we decided to combine three of them for subsequent refinement.![IMG_0779](https://user-images.githubusercontent.com/119873931/206718742-4cdd40b7-6cfc-46bf-a67e-d885b7bb9e95.JPG)
![IMG_0780](https://user-images.githubusercontent.com/119873931/206718751-738ecb00-8490-41d7-b77f-91526505439a.JPG)
I thought about three different solutions. One was about the relationship between the machine and nature and people, maybe through the vibration of metal pieces, the second was about Tamagotchi, and the third was about mechanical plants in the future. After discussion, we decided to do something about plant's rebirth.

### Inspiration:
People always want everything around them to exist the way people want it to, and living things including plants are being bound by people's wishes.
### The concept:
Whether machinery can be called "life" when it changes from a tool to assist human beings to a carrier to continue biological life, the process of "rebirth" is the gradual dissolution of a plant's own will, from symbiosis with machinery to its eventual replacement by complete mechanization. The project is an exploration of the possible collision and fusion between machinery and biology in the future, driven by the will of people. In choosing the main object for the installation, we were inspired by David Bowen's botanical installation recommended by our teacher and finally chose plants.
### Keywords: mechanical derivative, future technology, symbiosis
### Enclosure: 
mechanical branches protruding from plant branches, considering the use of dead plant branches hollowed out and connected to wobbling mechanical arms, other branches made entirely of machinery, with a metallic reflective surface
### Affordances: 
The branches connected to the plant sway in the direction of the human as he approaches, while the fully mechanical flowers are close to the human and open with touch rotation.
### Feedback: Feedback may be light, rotation, shaking, etc.
### Possible Input: touchboard, microphones, IR transistors, pressure
### Possible Output: motors, servo, muscle wire, stepper
Then I thought more carefully about the possibility of mechanical plants in the future：![IMG_0781](https://user-images.githubusercontent.com/119873931/206721242-f795511b-e300-4a4b-ba06-bc6f94ea9826.JPG)
# week 7:
### Goal this week: 
get a sense of which parts I would need, how I would use them, and get a general sense of how I could bring this project to life.

Through my research and interviews, I found that the risk of plant extinction is worse than before, and I investigated different people's views on how plants might exist in the future. People always want plants to be more resilient, to not need much care and to maintain a beautiful shape for a long time, so we discussed the idea that future plants could have stronger branches, when the machinery replaces the plant branches and has more positive feedback to people. So we designed a two-part branch and a mechanical flower.
Our device needed to take into account how the specific structure would be connected to the circuit, how the specific mechanical flower would rotate and open and how the robot arm underneath would be connected to the mechanical flower, and how the robot arm connected to the plant branch would move.
![IMG_7058](https://user-images.githubusercontent.com/119873931/206721972-03cd2175-4551-4605-9490-7e498e82cdf8.JPG)
I did a preliminary modeling of the flower part of the scheme, but it was quickly abandoned because we found a simpler and more efficient way to make it rotate and move up and down to achieve a flowering effect.
However, we soon realized that we needed to change the structure of the robot arm and the opening form of the mechanical flower, because there are many similar mechanical claws and soft mechanical arms with complicated structures on the web. After chatting with mett, who gave us advice, we finally chose to use three servo-driven robotic arms for our implementation, and we went to buy materials and chose to use laser cutting to make the parts for our robotic arms and the gears needed to rotate the flowers. For the gears we were going to use 3d printing, but unfortunately we didn't have a machine lined up, and we started to think about the material needed for the central support of the arm, and the way to connect the servos to the arm.
![IMG_2119](https://user-images.githubusercontent.com/119873931/206726394-3f7f062b-c5b7-4ea6-b40d-c44720636937.jpg)
![IMG_0783](https://user-images.githubusercontent.com/119873931/206726417-018816e9-a517-4ecd-82bf-5276080ef4e0.jpg)
# week 8:
Since it was a mechanically modified plant, we decided to make the branch part and the metal have a better combination, so for the shape of the branch I chose to use tin bending, this material is good for shaping and the surface of the metal shine is what I want. After the overall size of the device was determined I started to glue kitchen paper on the branches, which when glued and dried formed a fold on the surface of the branches, similar to the texture of tree bark, and while waiting for it to dry we determined that we needed five servos and a telescopic rod, two pressure sensors and a distance sensor. After testing we found that the laser cut material was heavy and we needed a larger voltage servo to support it, so we went and borrowed the needed material and started connecting the circuit.

The initial circuit we intended to use capacitor modules using one arduino board, but we had problems connecting them that didn't work and the solder connected boards always made poor contact, so we had to re-write the circuit using two arduino boards, leaving one connected to five servos, one distance sensor and one pressure sensor, and the other connected to one pressure sensor, the L298N board and the telescoping rod. We also need a 5v, a 12v and a rechargeable power supply, which means that our device needs to be left open for wiring.
![IMG_2D62B0DD80DC-1](https://user-images.githubusercontent.com/119873931/206727434-14c0030e-6881-48f2-b4c5-774b1d334cdb.jpeg)
In order to make the mechanical rod connected to the flower to be able to move closer to the direction when people are close, we repeatedly modified the angle of servo rotation so that it leaves space for the branch behind it when it moves. But after connecting the flower and the robot arm we encountered another problem. The value of the delay caused the flower to always wait for the robot arm to start moving after the person had already touched the pressure sensor, and it always responded too slowly for the overall effect to be good, so we kept the delay time of the flower and the robot arm the same, and they were able to move for a long time with little difference. Due to the change of the circuit, we had to re-solder the two boards, which took us longer.
![IMG_7354](https://user-images.githubusercontent.com/119873931/206727966-90a9c0fe-92e1-41aa-a3e6-00c567a50e43.JPG)
![IMG_7301](https://user-images.githubusercontent.com/119873931/206727979-6ea7a083-992f-459c-a097-083d6dddd16a.JPG)
![IMG_4CE6E63A8FE6-1](https://user-images.githubusercontent.com/119873931/206728151-007c1f9a-0a20-46c9-bea8-b7eb331d98eb.jpeg)
# week 9:
Building the device housing and circuit connections
We painted the branches wrapped in kitchen paper, and to make it more like a mechanical plant, we kept some metallic texture in the gaps of the branches, and we thought about how to connect the heavy robot arm and the flower inside the box and keep the three servos controlling the robot arm from interfering with the movement. We bought three different model clays, but the first time we bought the wrong one because it was hard to shape and dry. We then mixed the two types of milliput clay, made the base of the robot arm, and filled the clay around it to keep it in place, then hollowed out the partition to hide the electrical lines underneath 
### input: Pressure  Distance
### output: Servo Telescopic rod
![IMG_AE61B1196CD8-1](https://user-images.githubusercontent.com/119873931/206729437-c55dc430-ca58-4449-a439-624dde819d5d.jpeg)
![IMG_FE06C1E5A74F-1](https://user-images.githubusercontent.com/119873931/206729786-9a58905e-4db0-4b77-8a81-5abcfb7c0d9c.jpeg)
![IMG_2119](https://user-images.githubusercontent.com/119873931/206729838-0a39e320-f21d-4f60-9c60-c9bf1d9ae083.jpg)
### YOUTUBE LINK：https://youtu.be/L-8CkHXJ9do
