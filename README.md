# interims-tui
 A TUI program to visualize interim matches generated from University Advancement CRM. 
 TUI - is a Text based interface.  

![interims_tui](interims_tui.png) 

## Highlights
- ⚡️ Light and Fast
- 🖥️ Resource efficient
- 🛠️ Easily extensible


## Requirements 
#### Windows Terminal Emulator [](https://github.com/microsoft/terminal)
- Windows Terminal installers [Windows Terminal Releases](https://github.com/microsoft/terminal/releases/tag/v1.23.12811.0)
- Alternative Winget commandline installer
```powershell
winget install -e --id Microsoft.WindowsTerminal
```
#### Python 3.14 
- Download the the python installer. [Python install Link](https://www.python.org/ftp/python/3.14.0/python-3.14.0-amd64.exe)
- No winget link
- Other versions of python is unsupported

#### Installation
1) Download interims_tui
2) Navigate to the download directory
3) execute this command: 
```powershell 
pip install .\interims_tui-0.1.0-py3-none-any.whl
```

## Usage
To launch the program open up your terminal program, and launch interims-tui via: 
```powershell
 interims-tui
```

Navigate the application via clicking on the interim panel, and selecting a category, and a numbered item to display the contents. 
The application also allows naivagation via the keyboard arrow keys, and use the enter key to select.
Other commands are listed at the bottom of teriminal. 
Quit the application by clicking q on the keyboard, or closing the terminal


#### Configuration
After running interims-tui program you will have a configuration file made in your user folder. 
exmaple: C:\Users\dmv2s\.config\interims-tui\config.ini

Uncomment lines, by removing the comment indicator. '#'
Example:
```ini
[ucinn_ascendv2__Interim__c]
#Id # Record ID 
#OwnerId # Owner ID <-- to activate this field uncomment the first Number sign/hashtag symbol'#'
#IsDeleted # Deleted
```

```ini
[ucinn_ascendv2__Interim__c]
#Id # Record ID 
OwnerId # Owner ID <-- next load this field will show this field on the interim panel. Just hit r in the program to reload!
#IsDeleted # Deleted
```

The configuration file controls display of the interim object, and the Contac object. 
```ini
[ucinn_ascendv2__Interim__c] <-- This header shows which object you are configuring. 
# API Name # Label Name  <-- API name is the technical name of the field. The Label Name is what is displayed in the website. 
[contact]
# API Name # Label Name
```

