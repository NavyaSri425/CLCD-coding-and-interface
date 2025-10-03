# CLCD-coding-and-interface
Built a 16×2 character LCD demo using Arduino sketches and PicsimLab — completely simulated with no external hardware.  
It is useful for students and beginners to practice microcontroller coding and LCD interfacing virtually.
## 🚀 Features
- ✅ No external hardware required — fully simulated
- ✅ Arduino IDE for coding
- ✅ PicsimLab for circuit simulation
- ✅ 16×2 CLCD interfacing with LiquidCrystal library
- ✅ Demo video and screenshots included

## 💻 Code
```
#include <LiquidCrystal_I2C.h>
#include <wire.h>
LiquidCrystal_I2C lcd(0x27,16,2);
void setup() 
{
  lcd.init();          //Initialize the LCD
  lcd.backlight();     //Turn ON the back light
  lcd.clear();         //clear the CLCD screen
  lcd.home();          //set cursor to the first position on the CLCD

  lcd.setCursor(1,0);  //set Cursor at 0th line 1st column
  lcd.print("Hello");  

  lcd.setCursor(3,1);  //set cursor at 1st line 3rd column
  lcd.print("WELCOME ALL");
}
void loop() 
{
}
```
