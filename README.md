# Project done by Abinav Anantharaman and Satwik Shridhar Bhandiwad

# CS 5330 Spring 2023 --> Real Time Object Recognition 2D @ NEU

## Operating System and IDE:

I have used Ubuntu 20.04.5 LTS OS and Visual Studi Code 1.74.2 for this project. 
The IDE doesn't really matters because I have compiled and built the workspace using cmake and make terminal commands

### Installation of Dependencies
*  cmake,gcc and g++ installation
```bash
sudo apt install cmake gcc g++
```

### Workspace Installation
* Clone this workspace
```bash
cd [$Your_Destination_Folder]
git clone https://github.com/Abinav2695/PRCV_Project3_RTOR.git
```
* Build workspace
```bash
cd PRCV_Project3_RTOR/
mkdir build
cd build
cmake -S .. -B .
make
```

### Running Executables
* To run GUI application  
```bash
cd build
./bin/qt_gui {video source number} 
example -> ./bin/qt_gui 2  -->default 0
```


## Usage
Collect training data
Option 1 : Collect data using pre captured images.

Enter the csv file name by browsing the filepath to store training data.
Select the folder containing images of an object in different orientation in Train Database
field. Enter the label to be stored for this object. Ex: Soap_Box in the Object Label field.
Finally, click on Train Database button. This will compute the features and store in CSV.

Option 2: Collect training data from live feed.

Start the live feed for object detection by clicking start in the lower bottom corner.
When an unknown object arrives, enter the new label for this object in Object Label field and
click Save Feature Button. This will save the feature of this new object in the CSV file.

For Object Recognition

Start Cmaera Feed by clicking Start Button on lower bottom corner
Place the object under the camera frame on a white background
