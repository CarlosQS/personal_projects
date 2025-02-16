# Keylogger  

**Keylogger** is a straightforward tool for capturing keystrokes on Windows, Linux, and Mac. 

## Installation  

To install Keylogger using pip3, use one of the following commands:  

```bash
pip3 install -r requirements.txt
```
or

```bash
pip3 install pyxhook
```

## How to run it
Start logging keystrokes by running the command:
```bash
nohup python3 keylogger.py &
```
The nohup command stands for 'no hangup'. When used with &, the process continues running in the background without returning to the shell prompt
Example:
```bash
$ ~/Keylogger/linux$ nohup python3 keylogger.py &
[1] 12529  # This is the keylogger's PID (process ID)
$ ~/Keylogger/linux$ fg
```
The Keylogger is now actively recording keystrokes to a file.

## How to stop it
You can stop the Keylogger by:
- Typing the command fg and then pressing CTRL+C, or
- Using the kill command with the PID, for example:
```bash
kill 12529
```
