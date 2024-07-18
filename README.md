# SPR1NT3R-27-OPNSRC
this repo provides the documentation and firmware of the SPR1NT3R-27-OPNSRC printer. 

## Features

- **High-Quality Printing**: Delivers superior print quality with adjustable resolution settings.
- **Wireless Connectivity**: Supports Wi-Fi and Bluetooth connections for remote printing.
- **Multiple Paper Sizes**: Compatible with A4, A5, Letter, and Legal paper sizes.
- **Customizable Settings**: Allows customization of print speed, quality, and paper type.
- **Error Handling**: Advanced error detection and troubleshooting features.
- **Easy Of Use**: Easy to deal with interface update.

## Set-Up

After setting up your printer you have to connect it to the wifi 
### Printer Wi-Fi Connection and Interface Access

#### Connecting the Printer to Wi-Fi

1. **Power On**: Ensure the printer is powered on and ready.

2. **Access Settings**: Navigate to the Wi-Fi settings on the printer.

3. **Select Network**: Choose your Wi-Fi network and enter the password.

4. **Connect**: Save settings to connect the printer to Wi-Fi.

#### Accessing Printer Interface Using `nc` (Netcat)

1. **Find IP Address**: Locate the printer's IP address on your network.

2. **Open Terminal**: Launch a terminal window on your computer.

3. **Use `nc` Command**: Connect using:
   ```bash
   nc <printer_ip_address> <port_number>
   ```
## Menu
   The user has a menu of choices he can tweaker with.
   ![Screenshot 2024-07-18 150139](https://github.com/user-attachments/assets/428a49df-7892-4a41-9d95-b5020485dc22)

### Check Stats

   ![Screenshot 2024-07-18 150253](https://github.com/user-attachments/assets/bdca56ba-303d-4dcf-b8e2-e984d568e128)

## Commands

### Printing Commands

- `print <file>`: Print a specified file.
  ```shell
  print image.png
  ```
- `help`: displays the following menu:
  
  ![Screenshot 2024-07-18 144815](https://github.com/user-attachments/assets/b43a560b-65f8-448a-9f42-4aa4bf83219d)
- `set`: changes the state of a configuration variable
         

The XYZ Printer firmware repository is organized as follows:

- **`firmware/`**: Contains the main firmware files.
  - `main.cpp`: Entry point and main logic of the firmware.
  - `config.h`: Configuration settings for the printer.
  - `printer.cpp`, `printer.h`: Printer-specific functionalities.
  - ...

- **`docs/`**: Documentation files for the firmware.
  - `README.md`: Overview and instructions for using the firmware (this file).
  - `TROUBLESHOOTING.md`: Troubleshooting guide for common issues.
  - `CONTRIBUTING.md`: Guidelines for contributing to the project.
  - ...
