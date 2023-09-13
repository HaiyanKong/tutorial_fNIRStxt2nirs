# Convert the data recorded by SHIMADZU(.txt) to HOMER2 readable format (.nirs)

This repository is licensed under MIT.

## Step1: Prepare the followings

- MATLAB2013b

- [homer2](https://www.nitrc.org/plugins/mwiki/index.php/homer2:MainPage)

- [Shimadzu2nirs](https://www.nitrc.org/projects/shimadzu2nirs/)

## Step2: Set the path

Set **homer2**  in the path of MATLAB2013b.

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/1.png)

## Step3: Open the SDgui

- Set your work path at  *D:\toolbox\homer2\PACKAGES\SDgui* (change the path in the computer)

- Run **SDgui.m** in MATLAB2013b.

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/2.png)

- Next, a prompt will appear for you to select a file. Simply click "Cancel" to proceed.

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/3.png)

- Then you will see this.

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/4.png)

## Step4: Create the SD File

- Base on your optodes arrangement to fill in the blank in the sources and detectors.
  - Note: z is always 0.


![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/5.png)

- When you complete setting the sources and detectors , then click the number, you will get the channel.

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/6.png)

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/7.png)

- After setting channels, and you need to fill in the “Lambda” based on your data acquiring device.

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/8.png)

- Provide a name for the SD file, and let's call it "test.SD," including the ".SD" suffix.

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/9.png)

- Click the ''Save", and in the new window, you need to choose the "units", here is "mm"

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/10.png)

- Your SD file is saved successfully ! Just close the SDgui.

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/11.png)



## Step5: Convert!

- Put **the data need to convert (.txt)**, **3 files from Shimadzu2nirs.zip** and **test.SD created in step 4**  together, and set the MABLAB work path to them.

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/12.png)

- Run the **Shimadzu2nirs.m**, then you will get the **.nirs** data file !

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/13.png)

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/14.png)
