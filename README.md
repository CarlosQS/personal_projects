# Keylogger for Windows, Linux, and Mac  
[![MIT Licence](https://badges.frapsoft.com/os/mit/mit.png?v=103)](https://opensource.org/licenses/mit-license.php)  

This is a simple keylogger program designed to record keystrokes and save them to a log file on the local computer. It supports the three major operating systems: Windows, Mac, and Linux.  

## Contents  
- [Windows installation guide](https://github.com/GiacomoLaw/Keylogger/blob/master/windows/README.md)  
- [Mac installation guide](https://github.com/GiacomoLaw/Keylogger/blob/master/mac/README.md)  
- [Linux installation guide](https://github.com/GiacomoLaw/Keylogger/blob/master/linux/README.md)  
- [More information](https://simple-keylogger.github.io/)  

For more details, check the `README.md` file in each program's folder.  

## Windows  
To change the visibility of the window, modify the `#define` in line 13 to `visible` or `invisible`.  

Simply compile it into an `.exe` file and run it. Visual Studio is recommended for this.  

- `invisible`: Hides the keylogger window and starts it in the background. However, it is still visible in the task manager.  
- `visible`: The window remains open while typing, useful for testing.  

Both modes save keystrokes to a `.txt` file when the program is closed.  

> If you encounter compiler errors, try compiling again as the program should still work.  

## Mac  
For Mac users, refer to [this guide](https://github.com/caseyscarborough/keylogger).  

## Linux  

### Usage  
```bash
  pip install -r requirements.txt
  python3 keylogger.py
