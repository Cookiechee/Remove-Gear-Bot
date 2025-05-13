This is a tool that automates removing gear from characters in Last War: Survival using image recognition and Python automation.

🔧 How It Works

The "Bot":
- Searches for equipped gear using reference images
- Clicks the gear and presses the remove button
- Moves to the next character and repeats

💾 Setup Instructions

1. Place your gear images in the `/Images` folder (see file list below).
2. Configure settings in `config.ini`:
   - image_folder: path to the folder containing your reference images.
   - Toggle hotkey (default: F5)
   - The screen regions for gear, and remove button.
3. Run the bot using `remove_gear_bot.exe`

> ⚠️ Must be run as administrator for the hotkey to work!

🖱 Controls

- Press `F5` to start/pause the bot.
- Customize this key in `config.ini`.

📁 Included Files

- `remove_gear_bot.exe` — compiled bot
- `config.ini` — tweak hotkeys and screen coordinates
- `Images` — gear reference icons (`Radar.jpg`, `Gun.jpg`, etc.)

<pre> ``` Folder Structure: Remove Gear Folder
├── remove_gear_bot.exe     ✅ run this
├── config.ini              ✅ editable
└── Images
    ├── Radar.jpg
    ├── Armor.jpg
    ├── Gun.jpg
    ├── Chip.jpg
    ├── remove.png
    └── next.png    
 ``` </pre>
---

🧭 How to Find Your Screen Coordinates

If the bot isn’t clicking in the right place, you may need to update the screen coordinates in `config.ini`.

Here are some tools that can help you find them:

- 🧮 **[Microsoft PowerToys](https://learn.microsoft.com/en-us/windows/powertoys/)**  
  Shows your mouse position in real-time  
- 🎯 **[ShareX](https://getsharex.com/)**  
  Free tool with crosshair and coordinate tools
- 🔎 **Pixie** (very lightweight):  
  https://pixie.en.softonic.com/

---

🖼 Reference Image Tips
The bot uses pixel-perfect image matching, so your reference images must exactly match what’s on your screen.

If the default images don’t work:

🔍 Take your own screenshots of the gear, remove button, and next button

🖼 Crop them tightly around the icon (no extra space)

🚫 Avoid including gear level text or stars

🔁 Replace the files in the /Images folder


✅ Tips

- Make sure your game window stays in the same spot/size.
- By default this only works for UR/Gold gear.
- If detection fails, assume the image size/style differs — take your own screenshot
- Right click the exe - properties - compatibility - run as admin
