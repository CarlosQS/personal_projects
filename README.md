
# RecoverPy

RecoverPy is a robust utility that utilizes your system's features to recover lost data.

Unlike other tools, it can not only recover deleted files but also **overwritten** data.

It scans every block of your partition, and you can even search for specific strings within binary files.

* [Demo](#Demo)
* [Installation](#Installation)
    * [Dependencies](#dependencies)
    * [Run with pipx](#run-with-pipx)
    * [Installation from pip](#installation-from-pip)
    * [Installation from AUR](#installation-from-aur)
* [Usage](#Usage)
* [Tips](#Tips)


## Demo

<p align="center">
    <img src="docs/assets/demo.gif">
</p>

## Setup

:penguin: Currently, RecoverPy is available exclusively on Linux systems.  
:red_circle: **You need root access or to use sudo**.

### Dependencies

**Required:** To list and search through partitions, recoverpy relies on the `grep`, `dd`, and `lsblk` commands. These tools should already be present on most major Linux distributions.

**Optional:** To show real-time progress of the `grep` command, you can install `progress`.

To install the necessary dependencies:

- Debian-based: `apt install grep coreutils util-linux progress`
- Arch: `pacman -S grep coreutils util-linux progress`
- Fedora: `dnf install grep coreutils util-linux progress`

## Usage

### Run with uvx

`sudo uvx recoverpy`

### Run with pipx

`sudo pipx run recoverpy`

### Installation via pip

`python3 -m pip install recoverpy`

Then run `sudo python3 -m recoverpy`

---

- **Choose the system partition** where your file was stored. If you can't find it there, you can search your home partition, as sometimes your IDE or text editor may have made backups.

- **Enter a text string to search for**. See the tips below for better search results.

- **Start the search**, and the results will appear in the left-hand panel.

- **Pick a result**.

- Once you have found your file, **click `Open`**.

- You can now either save the block individually or explore adjacent blocks to find the remaining parts of the file. You can then save everything into one file.

## Tips

- Always make backups! Yes, we know, it's probably too late...
- **Unmount your partition before doing anything!** Although you can search with your partition mounted, it's highly recommended to unmount it first to prevent any accidental modifications to your file.

Regarding the search string:

- Keep it simple, try to use something unique to your file.
- Avoid using complex strings, as exotic characters may affect the search results.
- Try to remember the last changes you made to the file.

When you find your file:

- You may find multiple results. Your system often stores different versions of a file in separate partition blocks.
  Ensure you have located the most recent version.
- Explore surrounding blocks to confirm that you have recovered the entire file.
