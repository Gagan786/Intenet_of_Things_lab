The project, created by Gagan, involves an Arduino Nano 33 BLE Sense, a MiCS-4514 multi-gas sensor, an OLED screen, a fan, and a buzzer for sending out alerts.
The MiCS-4514 sensor is capable of detecting methane, ethanol, hydrogen, ammonia, carbon monoxide, and nitrogen dioxide.

To create this project, I followed these steps:

Collect data: Several samples were collected that ranged from typical to dangerous levels.
Train a neural network classifier: The dataset was fed into the Edge Impulse Studio to train a neural network classifier.
Calibrate the sensor: The device starts up, and the sensor is calibrated for a preset amount of time to distinguish harmful air.
Display sensor readings: The OLED screen shows any high sensor readings and indicates if a leak has been detected.

The project uses the MiCS-4514 multi-gas sensor, which can detect the following gases:
Methane (CH4) (1000–25000 PPM)
Ethanol (C2H5OH) (10-500 PPM)
Hydrogen (H2) (1-1000 PPM)
Ammonia (NH3) (1-500 PPM)
Carbon Monoxide (CO) (1-1000 PPM)
Nitrogen Dioxide (NO2) (0.1-10 PPM)

The device reads the gas sensor multiple times for a certain duration and then calculates the minimum, maximum, and average values for each gas. 
These values are used to train the neural network classifier and detect harmful gases in the environment.
