# circuitdigest
**Code for Eclipse**
**Step 1:** Setup the SSD1306 OLED Display
Assuming we are using the I2C interface, first need to set up the I2C communication and initialize the SSD1306 display.

**Step 2: **Adding the SSD1306 Library
We need to include or write a driver for the SSD1306 OLED display. Here’s a simplified version assuming a library is available:

**Step 3:** Integrate the OLED Display in the Access Control System
Modify the access control system to display relevant messages on the OLED display:

**Explanation:
**
**I2C Initialization:** The i2c_init() function sets up the I2C communication on the MAX78000. Adjust the I2C bus and address according to your setup.

**SSD1306 Initialization: **The ssd1306_init() function initializes the OLED display and clears it.

**Displaying Messages: **The display_message() function prints messages to the OLED display.

**Access Control Integration:** In the loop() function, the OLED display shows different messages depending on the face recognition result and the received password.

**Considerations:**
Ensure the SSD1306 driver is compatible with the setup and properly linked in the project.
If OLED uses SPI instead of I2C, modify the initialization and communication functions accordingly.
