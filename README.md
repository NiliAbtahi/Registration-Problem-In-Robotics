# Registration-Problem-In-Robotics

The aim is, in this algorithm, to find Euclidean transformation between two coordinate systems for given position vectors of some points in the one system and their correspondence in the other. The formalism is based on a least square problem that is explaned in full detail in the documentation PDF file in the docs folder. 

Also a Matlab code is provided for implemting the algorithm.  The main.m file drives the program by taking two arrays of 3D position vectors in the two coordinate systems and then calling the function data_registration in the m-file with the same name. Some smaples for input data are provided in the test-data folder. 

## How To Use Code
* Download/clone the repository 
* Open Matlab/Octave software and navigate it to the folder containing the m-files
* In Matlab/Octave command window write:
```Matlab
   main   firstFile.txt   secondFile.txt
```
where the text files have a format similar to those in the test-data folder
* You can also directly call the data_registration function in command window by
```Matlab
   data_registration( first_system_3D_points , second_system_3D_points )
```
   where the arguments are arrays of position vectors of 3D points in two coordinate systems.

### Example for smaples in the test-data folder
```Matlab
   main   ./test/data1-firstFrame.txt   ./test/data1-secondFrame.txt
   main   ./test/data2-firstFrame.txt   ./test/data2-secondFrame.txt
   main   ./test/data3-firstFrame.txt   ./test/data3-secondFrame.txt
```
