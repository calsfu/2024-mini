# Miniproject Answers

## Exercies

### Exercise 01
#### Questions
1. We found that a max brightness of 21000 and a minimum brightness 7000 worked well for calibrating our led. In our testing, the light turned off in bright conditions and turned on in dark conditions, and had a noninteger duty cycle in between.

### Exercise 02
1. We modified the code to play a rendention of the Super Mario Bros. theme. 

### Exercise 03
1. We edited the code to compute the average, minimum, and maximum response time for 10 flashes.
2. We uploaded the response time data to a realtime Firebase database. First, the raspberry pi connects to the BU guest wifi using the network library. Then data is then sent to the database using a POST request with the requests library. In order to ensure that only our data is being sent to the database, we used a unique key that is only known to us. The key is stored in a json file in the raspberry pi. To load a new key, the key must be added to main with the `load_json` function uncommented. 