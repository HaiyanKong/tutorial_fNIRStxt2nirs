# Convert the data recorded by SHIMADZU(.txt) to HOMER2 readable format (.nirs)

## Step1: Prepare the followings

MATLAB2013

homer2[https://www.nitrc.org/plugins/mwiki/index.php/homer2:MainPage]

Shimadzu2nirs [https://www.nitrc.org/projects/shimadzu2nirs/]

## Step2: Set path

put homer2 at the path of MATLAB2013

## Step3: Open the SDgui

run SDgui.m in MATLAB2013

- note: SDgui.m is here →[...\homer2\PACKAGES\SDgui\SDgui.m]

then you will get this UI

1.png

## Step4: Set your sources, detectors and channels in SDgui

base on your experiment setting and data acquiring device fill the blank in the red box

- note1: z is always 0

- note2: when you finish the sources and detectors setting, click the middle of them, you will get the channel

2.png

then save your SD File

3.png

## Step5: Convent!

put your data(.txt), three files in Shimadzu2nirs.zip and .SD file together

4.png

then run the Shimadzu2nirs.m, you will get the data.nirs!

5.png
