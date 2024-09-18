# Miniproject Answers

## Exercises

### Exercise 01
#### Questions
1. We found that a max brightness of 21000 and a minimum brightness 7000 worked well for calibrating our led. In our testing, the light turned off in bright conditions and turned on in dark conditions, and had a noninteger duty cycle in between.


https://github.com/user-attachments/assets/8957fc7a-2dba-4bc7-a213-44a945387a5e


### Exercise 02
1. We modified the code to play a rendention of the Super Mario Bros. theme. 


https://github.com/user-attachments/assets/f429c421-7400-4741-ae07-ecd3a5418a01


### Exercise 03

#### User Story
As a player of the flash game, I would like my game metrics to be stored on the cloud, so I can access them easily from any device, and my metrics won't be erased, if the raspberry pi pico gets reset.
As a developer of the flash game, I would like game metrics to be stored on the cloud, so I can centralize each players game metrics and query info based on each player when needed. Storing information on the cloud also means that only authorized users can read and write data. For example, one player cannot change another player's data.


1. We edited the code to compute the average, minimum, and maximum response time for 10 flashes.
2. We uploaded the response time data to a realtime Firebase database. First, the raspberry pi connects to the BU guest wifi using the network library. Then data is then sent to the database using a POST request with the requests library. In order to ensure that only our data is being sent to the database, we used a unique key that is only known to us. The key is stored in a json file in the raspberry pi. To load a new key, the key must be added to main with the `load_json` function uncommented. The rule to only let authorized users read and write to the database is specified under the rules tab of the Firebase realtime database console. The rules metrics under the usage tab on the console also shows that 5 reads/writes were denied successfully. In our demo video, we have four entries of game data each including the average, minimum, and maximum response time from 4 rounds of playing the game.



https://github.com/user-attachments/assets/f853e6f5-74a2-4201-ba1d-714bb190540e



