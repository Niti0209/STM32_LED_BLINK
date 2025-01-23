# STM32 Projects 
## **Project 1: Onboard LED Blinking**

### **Objective**
Create a program to make the onboard LED blink with a delay of 500ms.

### **Steps**
1. **Setup STM32CubeIDE:**
   - Install and configure the STM32CubeIDE.
   - Create a new STM32 project and select the appropriate board using the Board Selector option.

2. **Configure GPIO Pins:**
   - Use the configuration tool to set up the GPIO pin connected to the onboard LED.

3. **Code Implementation:**
   - Edit the `main.c` file and make the following changes:
     ```c
     while (1) {
         HAL_GPIO_WritePin(GPIOA, GPIO_PIN_5, GPIO_PIN_SET);
         HAL_Delay(500);
         HAL_GPIO_WritePin(GPIOA, GPIO_PIN_5, GPIO_PIN_RESET);
         HAL_Delay(500);
     }
     ```

4. **Build and Run:**
   - Build the project and run it to observe the LED blinking at a 500ms interval.

---


## **How to Use This Repository**
1. Clone the repository:
   ```bash
   git clone <repository-link>
   ```
2. Open the project in STM32CubeIDE.
3. Follow the instructions in the respective project folder to set up and run the code.

---

Feel free to reach out for any questions or suggestions! 😊
