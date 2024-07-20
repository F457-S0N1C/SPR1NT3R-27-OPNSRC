# SPR1NT3R-27-OPNSRC
this repo provides the documentation and server files of the SPR1NT3R-27-OPNSRC printer. 

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
   ![Screenshot 2024-07-20 105736](https://github.com/user-attachments/assets/50e52892-aa20-49eb-9277-68b0d1190333)

### Check Stats

   ![Screenshot 2024-07-20 105612](https://github.com/user-attachments/assets/598ff13c-763c-41df-b9d8-3956af548639)


## Commands

### Printing Commands

- `print <file>`: Print a specified file.
  ```shell
  [-] > print image.png
  ```
- `print -l`: Displays all the files in the image directory.
  ```shell
     [-] > print -l 
      └──images/
         └───sonic.png✔️
  ```
- `help`: displays the following menu:
  
  ![Screenshot 2024-07-18 144815](https://github.com/user-attachments/assets/b43a560b-65f8-448a-9f42-4aa4bf83219d)
- `set`: changes the state of a configuration variable
  ```shell
  set commands enable <password>
  ```
  *PS: password is not always required
         

## File Structure
- **`src/`**: Contains the main source code and files.
  - `server.py`: The server source code.
  - `supersecret.png`: Contains the default password for the configuration permission.
  - `sonic.png`: A test image provided with the server by default.
## Feedback
   Please don't hesitate to send your feedback on the challenge upon completion.

