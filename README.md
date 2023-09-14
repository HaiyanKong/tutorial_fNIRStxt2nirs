# Convert the data recorded by SHIMADZU(.txt) to HOMER2 readable format (.nirs)

This repository is licensed under MIT.

## TOC

-   [1. Convert tutorial](#Conver-tutorial)
-   [2. The common error](#The-common-error)



## Convert tutorial

### Step1 Prepare the followings

- MATLAB2013b

- [homer2](https://www.nitrc.org/plugins/mwiki/index.php/homer2:MainPage)

- [Shimadzu2nirs](https://www.nitrc.org/projects/shimadzu2nirs/)

### Step2: Set the path

Set **homer2**  in the path of MATLAB2013b.

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/image/1.png)

### Step3: Open the SDgui

- Set your work path at  *D:\toolbox\homer2\PACKAGES\SDgui* (change the path in the computer)

- Run **SDgui.m** in MATLAB2013b.

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/image/2.png)

- Next, a prompt will appear for you to select a file. Simply click "Cancel" to proceed.

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/image/3.png)

- Then you will see this.

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/image/4.png)

### Step4: Create the SD File

- Base on your optodes arrangement to fill in the blank in the sources and detectors.
  - Note: z is always 0.


![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/image/5.png)

- When you complete setting the sources and detectors , then click the number, you will get the channel.

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/image/6.png)

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/image/7.png)

- After setting channels, and you need to fill in the “Lambda” based on your data acquiring device.

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/image/8.png)

- Provide a name for the SD file, and let's call it "test.SD," including the ".SD" suffix.

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/image/9.png)

- Click the ''Save", and in the new window, you need to choose the "units", here is "mm"

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/image/10.png)

- Your SD file is saved successfully ! Just close the SDgui.

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/image/11.png)

### Step5: Convert!

- Put **the data need to convert (.txt)**, **3 files from Shimadzu2nirs.zip** and **test.SD created in step 4**  together, and set the MABLAB work path to them.

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/image/12.png)

- Run the **Shimadzu2nirs.m**, then you will get the **.nirs** data file !

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/image/13.png)

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/image/14.png)



## The common error

If the optodes arrangement of your experiment is as follows:

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/error/1.png)

Then your SD file arrangement must correspond one-to-one:

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/error/2.png)

If the arrangements are totally inconsistent, for example:

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/error/3.png)

The error will be:

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/error/4.png)

If the arrangements are consistent but the channel numbers in the SD file are inconsistent, for example:

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/error/5.png)

The error will be:

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/error/6.png)

