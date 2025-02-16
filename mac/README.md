## Mac  
This version is a bit more complex (it's Apple, after all). It doesn't work in secure input fields like password prompts. Currently, no workaround has been found for this.  

### Installation  
Begin by downloading the repository. It will install to `/usr/local/bin/keylogger`.  

To install it, run the following commands:  

```bash
$ git clone https://github.com/GiacomoLaw/Keylogger && cd keylogger/mac
$ make && make install
```
By default, keystrokes will be logged to `/var/log/keystroke.log`. This might need root permissions, but you can change the log location if desired:
```bash
$ keylogger ~/logfile.txt
Logging to: /var/log/keystroke.log
```
Want it to start automatically when the system boots? Use:
```bash
$ sudo make startup
```
This will enable it to run at startup

## Uninstall
To remove the program (but not the logs), run:
```bash
$ sudo make uninstall
```
