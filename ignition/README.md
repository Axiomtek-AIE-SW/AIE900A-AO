# Smart Ignition Management
To access the Smart Ignition Management main menu, please enter the following command in the terminal:  
`$ psu2_axiomtek.sh`

Brief information about the current settings will be displayed at the bottom of the main menu:
 - **FW Version:** Current firmware version
 - **Ignition Management:** Enabled or Disabled
 - **Auto Power On:** Enabled or Disabled
 - **Vin Voltage:** Current Vin Voltage
 - **IGN Signal:** Current Ignition Signal (On or OFF)  
![image](https://github.com/user-attachments/assets/e18bb709-e70d-4731-a33e-1fb77b77fc42)

The Smart Ignition Management menu enables users to configure settings related to the vehicle ignition switch. The relevant ignition status setting values are displayed below:  
## a. The current setting
To view the detailed threshold settings of Smart Ignition, including the following items:
- Power-on Voltage (System powers on when voltage reaches this level)
- Undervoltage (System shuts down if voltage drops below this level)
- Undervoltage shutdown delay timer (if low voltage continues for the period)
- Ignition power-on delay timer (a delay when the ignition signal is detected)
- Ignition shutdown delay timer (a delay when the ignition signal is lost)

## b.	Ignition Management
- To enable or disable the function of Smart Ignition Management.
- To return to the main menu, select **"Cancel"**.

## c.	Advanced Settings
### 1)	Auto Power On Mode
To enable or disable Auto Power On Mode

### 2)	Power-On/Undervoltage Detection  
#### 2-1)	Power-On and undervoltage voltage threshold configuration  
To adjust the voltage value of undervoltage voltage threshold value (Range from 9.0 to 23.0V) and power-on voltage threshold value (Range from 9.0 to 24.0V)  
#### 2-2)	Undervoltage shutdown delay timer  
To adjust the undervoltage shutdown delay EndTime value (Range from 60 to 10800 seconds)  

### 3)	Ignition Power Delay  
#### 3-1)   Power-On Delay Timer  
To adjust Power-On delay EndTime value (Range from 2 to 1800 seconds)  
#### 3-2)	Shutdown Delay Timer:  
To adjust shutdown delay EndTime value (Range from 1 to 21600 seconds)  

### 4)	Cancel
To return to the main menu, select **"Cancel"**.  

## d.	Save Setting (Saves changes as the custom default)
To immediately save changes as the custom default, select **"d"** from the main menu. **“Save Settings …[OK]”** will be displayed once the saving process is complete.

## e.	Restore Default Setting
- To restore custom default or factory default from the EEPROM. **“Restore Custom Default …[OK]”** or **“Restore Factory Default…[OK]”** will be displayed once the restoration process is complete.
- To return to the main menu, select **"Cancel”**.

## x.	Exit
To exit the Smart Ignition Management main menu, select **“x”**.  

# View detailed current settings of Smart Ignition
**Step 1.** Access the Smart Ignition Management main menu.  
**Step 2.** Select **“a”**. The detailed current settings of Smart Ignition will be displayed, and the system will automatically return to the main menu afterward.  
![image](https://github.com/user-attachments/assets/d41d9636-7ec3-42aa-9d4e-d42430ef6749)

# Switch of the Smart Ignition Function
**Step 1.** Access the Smart Ignition Management main menu.  
**Step 2.** Select **“b”**.  
**Step 3.**
- **To enable Smart Ignition Management:**  
Select **“1”** and the system will automatically return to the main menu afterward.
- **To disable Smart Ignition Management:**  
Select **“2”** and the system will automatically return to the main menu afterward.
- **To exit without making changes:**  
Select **“3”** to return directly to the main menu.  
![image](https://github.com/user-attachments/assets/81460a98-032c-40f3-b831-b81272d21f38)

# Auto Power On Mode Setting
**Step 1.** Access the Smart Ignition Management main menu.  
**Step 2.** Select **“c”**.  
**Step 3.** Select **“1”** to open the Auto Power On Mode menu.  
**Step 4.**
- **To enable Auto Power On Mode:**  
Select **“1”** and the system will automatically return to the main menu afterward.
- **To disable Auto Power On Mode:**  
Select **“2”** and the system will automatically return to the main menu afterward.
- **To exit without making changes:**  
Select **“3”** to return directly to the main menu.  
![image](https://github.com/user-attachments/assets/1b9636f1-e32e-43b7-88d7-c7fd8db2b830)

# Power-On/Undervoltage Detection Settings
**Step 1.** Access the Smart Ignition Management main menu.  
**Step 2.** Select **“c”**.  
**Step 3.** Select **“2”** to open the Power-On/Undervoltage Detection menu.  
**Step 4.**  
- **To configure power-on and undervoltage voltage thresholds:**  
Select **“1”** then follow the on-screen instructions to enter the desired values, and the system will automatically return to the main menu afterward.
- **To exit without making changes:**  
Select **“3”** to return directly to the main menu.  
![image](https://github.com/user-attachments/assets/a18c5725-95da-4b12-8678-931f85efbcae)

# Power-On/Undervoltage Detection Setting
**Step 1.** Access the Smart Ignition Management main menu.  
**Step 2.** Press **“c”**.  
**Step 3.** Select **“2”** to access the Power-On/Undervoltage Detection menu.  
**Step 4.**
- **To adjust the undervoltage shutdown delay timer:**  
Select **“2”** then follow the on-screen instructions to enter the desired value, and the system will automatically return to the main menu afterward.
- **To exit without making changes:**  
Select **“3”** to return directly to the main menu.  
![image](https://github.com/user-attachments/assets/3dabb83b-c604-49fc-be63-b379fcf452d5)

# Ignition Power Delay – Power-On Delay Timer
**Step 1.** Access the Smart Ignition Management main menu.  
**Step 2.** Select **“c”**.  
**Step 3.** Select **“3”** to open the Ignition Power Delay menu.  
**Step 4.**
- **To configure the Power-On Delay Timer:**  
Select **“1”** then follow the on-screen instructions to enter the desired value, and the system will automatically return to the main menu afterward.
- **To exit without making changes:**  
Select **“3”** to return directly to the main menu.  
![image](https://github.com/user-attachments/assets/1871bbf5-2107-4673-ace5-165c49b8c47b)  
![image](https://github.com/user-attachments/assets/96a560f2-8f0f-4b6b-b19b-77690af4e516)

# Ignition Power Delay – Shutdown Delay Timer
**Step 1.** Access the Smart Ignition Management main menu.  
**Step 2.** Select **“c”**.  
**Step 3.** Select **“3”** to open the Ignition Power Delay menu.  
**Step 4.**
- **To configure the Shutdown Delay Timer:**  
Select **“2”** then follow the on-screen instructions to enter the desired value, and the system will automatically return to the main menu afterward.
- **To exit without making changes:**  
Select **“3”** to return directly to the main menu.  
![image](https://github.com/user-attachments/assets/dadf6e2c-a26a-4710-894b-a27251ee97b8)  
![image](https://github.com/user-attachments/assets/bc7d1ff4-003a-411b-b77f-035476988d30)

# Save Setting - Saves Changes as the Custom Default
*★	Executing this option will save all the changes you made in the Smart Ignition Management menu as **custom defaults.**  
To ensure the custom defaults are applied when the system is powered off, you must execute this option before exiting the Smart Ignition Management menu. If you do not, the current settings will be lost after power-off, and the system will revert to the last saved presets.*  
**Step 1.** After making all desired changes, return to the Smart Ignition Management main menu.  
**Step 2.** Select **“d”**.  
**Step 3.** The system will save your changes as custom defaults. **“Save Settings…[OK]”** will appear once the saving process is complete, and the system will automatically return to the main menu afterward.  
![image](https://github.com/user-attachments/assets/523e0ebe-3506-40a6-bcac-4796a9fb4605)  

# Restore Default Setting
*★	Executing this option will immediately restore the default settings (either custom default or factory default) of Smart Ignition Management.*   
**Step 1.** Access the Smart Ignition Management main menu.  
**Step 2.** Select **“e”**.  
![image](https://github.com/user-attachments/assets/c1aa88e2-c8bd-4e81-b053-dabcd6a27872)  
**Step 3.**
- **To restore the custom default from EEPROM:**  
Select **“1”**; “*Restore Custom Default…[OK]*” will appear once the process is complete, and the system will automatically return to the main menu afterward.  
![image](https://github.com/user-attachments/assets/14c0800c-8675-43d7-be35-f8c57c136df9)  
- **To restore the factory default from EEPROM:**   
Select **“2”**; “*Restore Factory Default…[OK]*” will appear once the process is complete, and the system will automatically return to the main menu afterward.  
![image](https://github.com/user-attachments/assets/638e588d-2c79-4ac3-ac32-a0bc55443dbe)
- **To exit without making changes:**  
Select **“3”** to return directly to the main menu.
