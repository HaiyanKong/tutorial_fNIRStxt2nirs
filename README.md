# Convert the data recorded by SHIMADZU(.txt) to HOMER2 readable format (.nirs)

This repository is licensed under MIT.

## Step1: Prepare the followings

- MATLAB2013b

- [homer2](https://www.nitrc.org/plugins/mwiki/index.php/homer2:MainPage)

- [Shimadzu2nirs](https://www.nitrc.org/projects/shimadzu2nirs/)

## Step2: Set path

Put **homer2** at the path of MATLAB2013b.

## Step3: Open the SDgui

- Run **SDgui.m** in MATLAB2013b.

  - SDgui.m   → *...\homer2\PACKAGES\SDgui\SDgui.m*

Then you will see this UI: 

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/1.png)

## Step4: Set your sources, detectors and channels in SDgui

Base on your experiment setting and data acquiring device fill the blank in the red box.

- Note1: z is always 0.

- Note2: when you finish the sources and detectors setting, click the middle of them, you will get the channel.

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/2.png)

Save your **SD File**.

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/3.png)

## Step5: Convert!

Put the **data(.txt)**, **three files from Shimadzu2nirs.zip** and **.SD file** created just now together

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/4.png)

Run the **Shimadzu2nirs.m**, then you will get the **data.nirs**!

![image](https://github.com/HaiyanKong/Convert-data.txt-to-data.nirs/blob/main/5.png)
