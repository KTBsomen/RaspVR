## **RaSVR - VRSAT**
				Radio Spectrum Visualizer and recorder - VLF Radio Signal Analysis Tool
# VRSAT
so **VRSAT** is the second step of our VLF toolkit, in this program we plot signal data from our recorder program(**RaSVR**) 
we record the data of VTX and NWC transmitter 
in the following demo format the column names are in order of don't include column names in actual data

		year	time	  VTX    NWC

    2023-01-14 00:00:00 -53.89 -74.69
    2023-01-14 00:00:00 -53.82 -74.38
    2023-01-14 00:00:00 -53.8 -74.58
    2023-01-14 00:00:01 -53.94 -74.81
    2023-01-14 00:00:01 -53.98 -74.67
    2023-01-14 00:00:01 -54.01 -74.51
    2023-01-14 00:00:02 -53.96 -74.58
    2023-01-14 00:00:02 -53.79 -74.78
    2023-01-14 00:00:02 -53.66 -74.85
    2023-01-14 00:00:03 -53.77 -75.42
    2023-01-14 00:00:03 -53.96 -75.3
    2023-01-14 00:00:03 -53.81 -74.91
    2023-01-14 00:00:04 -53.8 -75.53
    2023-01-14 00:00:04 -53.69 -75.49
    2023-01-14 00:00:04 -53.78 -75.58
    2023-01-14 00:00:05 -53.78 -75.22

OR with microsecond accuracy 

    2023-01-14 00:00:0.0 -53.89 -74.69
    2023-01-14 00:00:0.0 -53.82 -74.38
    2023-01-14 00:00:0.0 -53.8 -74.58
    2023-01-14 00:00:0.1 -53.94 -74.81
    2023-01-14 00:00:0.1 -53.98 -74.67
    2023-01-14 00:00:0.1 -54.01 -74.51
    2023-01-14 00:00:0.2 -53.96 -74.58
    2023-01-14 00:00:0.2 -53.79 -74.78
    2023-01-14 00:00:0.2 -53.66 -74.85
    2023-01-14 00:00:0.3 -53.77 -75.42
    2023-01-14 00:00:0.3 -53.96 -75.3
    2023-01-14 00:00:0.3 -53.81 -74.91
    2023-01-14 00:00:0.4 -53.8 -75.53
    2023-01-14 00:00:0.4 -53.69 -75.49
    2023-01-14 00:00:0.4 -53.78 -75.58
    2023-01-14 00:00:0.5 -53.78 -75.22
Here is a demo file of Raw Data [Click to Download rawdata ](https://drive.google.com/uc?export=download&id=1SekzDxAvRgix5ran9zYQIwLDuhA7iOR1)

after we record the data in a file we will load the data in our **VRSAT** software to analyze it
to do so first 

 - download our **VRSAT** software open it
 - Open the software
 - Click on the Add Folder Button at the top left
 - select the folder in which you have stored the data files 
 - after selecting the folder you can see all of your files listed on the software 
 - click on any file you want to plot and analyze
 - The contents of the file will be show in the right panel (**READ ONLY**)
 - then below you can see some check boxes 

 - [ ] VTX
 - [ ]  NWC
 - [ ] RAW
 - [ ]  Minute Average
 - [ ] Rolling Average

After the Rolling Average filed one can see a input field with default value of 39 this value is the window length like how much data to be consider in one iteration
and then you will see **View Plot** button 
and next to it you can see **(?)**  this is for help
![look of VRSAT by somen6562@gmail.com somen das](https://drive.google.com/uc?export=download&id=13QXetgdb4DfnqkuLilL6ZtgzDKLc3YWx)

# now to plot specific data use combinations of the check boxes 
 - [x] NWC 
 - [x] RAW
**View Plot**
this combination will produce a plot of raw VTX data
![nwc raw data ](https://drive.google.com/uc?export=download&id=1gzqrsrFk32A5KTFMDRPIHMzV5VMHZ0QY)
#
 - [x] NWC 
 - [x] Minute Average
**View Plot**
this combination will plot Minute Average of NWC data
![minute average of nwc](https://drive.google.com/uc?export=download&id=1IIJQISEhD7VCK6IKiPIO7qUNVKkld6nx)
#
 - [x] NWC 
 - [x] VTX
 - [x] Minute Average
**View Plot**
this combination will plot Minute Average of NWC and VTX data
![Minute Average of NWC and VTX](https://drive.google.com/uc?export=download&id=1lfAGdKQ-Ptsgk_2wnzW0mwzZbsulbNvS)
#
Whenever You Plot Minute Average the data will be stored in your selected folder with name like

    [Raw File Name].mint[nwc or vtx].txt
    like this 14012023.txt.mintnwc.txt

