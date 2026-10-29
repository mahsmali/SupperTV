[README.txt](https://github.com/user-attachments/files/34154684/README.txt)
SUPER TV - installable Samsung TV app
=====================================

What this is
  SUPER TV packaged as a real Samsung (Tizen) TV app. Once installed it lives on the TV:
  no phone, no website hosting and no browser needed to open it. Fonts are built in, so
  the app itself works offline (websites and streaming apps still need the internet).

What you need (all free)
  - A Windows, Mac or Linux computer on the same Wi-Fi as the TV (only for installing, about 30-45 minutes once)
  - Tizen Studio from developer.tizen.org, with the "TV Extensions" and "Samsung Certificate Extension"
  - A free Samsung account
  - Your TV's address: 192.168.1.116 (already written into both install scripts)

Steps
  1. Install Tizen Studio. In its Package Manager, open "Extension SDK" and install
     "TV Extensions" and "Samsung Certificate Extension".
  2. Find your computer's own IP address (Windows: run ipconfig; Mac: System Settings > Wi-Fi > Details).
  3. On the TV: open Apps, then enter 1 2 3 4 5 with the remote (Smart Remote: press the 123 button
     for the on-screen number pad). Switch Developer Mode ON, type your COMPUTER's IP, OK.
     Turn the TV fully off and on (hold the power button).
  4. In Tizen Studio: Tools > Device Manager > Remote Device Manager > + > IP 192.168.1.116, port 26101,
     then switch the connection on. The TV appears in the list.
  5. Tools > Certificate Manager > + > Samsung > TV. Name the profile exactly: SuperTV
     Create a new author certificate (any name and password you choose), sign in with your Samsung
     account, keep the default distributor settings and make sure your TV's DUID is listed. Finish.
  6. Run install-supertv-windows.bat (Windows) or install-supertv-mac-linux.sh (Mac/Linux).
     If Tizen Studio is not in the default folder (C:\tizen-studio or ~/tizen-studio), edit TS= in the script.
  7. On the TV press Home: SUPER TV is in the apps bar. Highlight it, press Down, choose Move,
     and put it first.

Make it start with the TV (closest to "permanent")
  Leave SUPER TV open when you switch off, and turn on "Autorun Last App" if your TV's menu has it
  (2024 models: Settings > All Settings > General & Privacy > Start Screen Option). The TV then reopens
  the last app at power-on. Menu names vary by software version.

After installing
  You can switch Developer Mode off again (Apps > 1 2 3 4 5). SUPER TV stays installed.
  If a future TV update ever removes it, run the install script again.

What it cannot do
  No app, including this one, can replace Samsung's Smart Hub, change firmware, or show live TV
  channels without Samsung partner permissions. Apps it opens follow your normal subscriptions.

Font licences: fonts/OFL-*.txt (SIL Open Font License).
