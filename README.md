# sway-alt-tab

This script adds `Alt-Tab` functionality to Sway, allowing you to switch between two containers. Here's how it works:

- **Select Containers:** Hold down `Alt` and navigate to the container you want to switch to. 
- **Switching:** Release `Alt` when you've selected your desired container. 
- **Direct Use:** You can also use `Alt-Tab` directly without releasing `Tab`, and the script will remember the second container ID for switching.

## Setup

### 1. Sway Config

Add the following lines to your Sway configuration file (`~/.config/sway/config`):

```text
# For alt-tab functionality
bindsym --no-repeat Alt_R exec /path/to/script/alt-tab save
bindsym --no-repeat Alt_L exec /path/to/script/alt-tab save
bindsym --no-repeat $mod+Tab exec /path/to/script/alt-tab switch
```

## 2. Download and Setup Script

- **Download:** Download Script.
- **Make Executable:** Change the script's permissions to make it executable:
 `chmod +x /path/to/script/alt-tab`
