# USBConsole-FWGenerator
## Folder Structure 
**App_Combine_BL_Generator:** Application folder that contains bootloader, json keys, encryption .exe file, python script for combining bootloader and encrypted firmware  
**App_No_BL_Generator:** Application folder that contains json keys and encryption .exe file  
**FW_Combine_BL:** Output folder that contains the generated combined encrypted firmware with bootloader  
**FW_No_BL:** Output folder that contains the generated encrypted firmware without bootloader  
**FW_Only:** Input folder that contains the original version of the firmware binary  
## How to Generate Firmware 
1. Run USBConsole-FWGenerator.bat script  
2. User is required to select the firmware generator of choice 
```
1 - No_BL_Generator : Generate encrypted firmware without bootloader
2 - Combine_BL_Generator : Generate encrypted firmware combined with bootloader
```
3. Type option '1' or '2' and press enter
4. A pop out window will show for user to browse the input folder path and select the original firmware binary file 
5. Select the original firmware binary file
6. Summary of the firmware generator details and process will be shown on terminal 
```
DEBUG - Parameter values: 
FWNAME: Input original firmware binary file name
INPUTDIR: Path to original firmware binary file directory
EXEFILE: Firmware encryption .exe file name
GENERATORDIR: Path to firmware generator directory
OUTPUTFILE: Output generated firmware binary file name
OUTPUTDIR: Path to output firmware binary directory
```
7. Terminal will show this message upon successful firmware generation process - else error log message will be shown
```
Checksum generation complete.
Encryption complete.
Press any key to exit.
```
8. To exit program, press enter 
9. Exit program will automatically open the specific output folder where the generated output binary file can be found
