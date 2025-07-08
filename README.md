# Home-Automation-with-Bluetooth
DESIGN A BLUETOOTH-CONTROLLED HOME AUTOMATION SYSTEM TO SWITCH DEVICES ON AND OFF
✅ Project: Bluetooth-Controlled Home Automation
🔧 Components Required:
Arduino UNO/Nano

HC-05 Bluetooth module

2-channel Relay module (or more)

Android phone with Bluetooth Terminal App (e.g., Serial Bluetooth Terminal)

5V power supply

Loads (bulb/fan simulated with LEDs or real AC devices)

📲 System Overview:
User sends command via mobile app over Bluetooth.

Arduino receives the command and controls relays to turn devices ON/OFF.

🔌 Wiring Diagram:
Component	Arduino Pin
HC-05 TX	RX (Pin 0)
HC-05 RX	TX (Pin 1) (via voltage divider)
HC-05 VCC	5V
HC-05 GND	GND
Relay IN1	D8
Relay IN2	D9
Relay VCC/GND	5V / GND

⚠️ Use a voltage divider (1kΩ + 2kΩ) for HC-05 RX line, as it's 3.3V-tolerant. 

📱 Phone App Commands:
You can use any Bluetooth terminal app to send the following commands:

A → Turn ON device 1

a → Turn OFF device 1

B → Turn ON device 2

b → Turn OFF device 2

💡 You can build a custom app using MIT App Inventor or use prebuilt apps like “Bluetooth Terminal”.

⚙️ Working Explanation:
Power on Arduino and pair HC-05 with your phone.

Open Bluetooth terminal and send characters like A, a, B, or b.

Arduino reads data and toggles relays, which control connected appliance





