# ecd
===
A extention tool to manage your working path list
### Help page
```sh
$ ecd -h
ecd [ -i | -b [Index] | -s | -l | -h | -r [Index] | -[Index] | [DIRECTORY] ]
       -i: interactive mode
       -b: branch mode, [Index]: 0..Current History Count
       -l: list the history
       -s: sort list
       -h: display this information
       -r: remove a certain index
       -[NUMBER]: go to index NUMBER
       [DIRECTORY]: go to DIRECTORY

```
### Installation
0. copy the script to your home directory
```sh
$ mv bashrc_ecd ~/.bashrc_ecd
```
1. add following line to your ~/.bash_profile or ~/.bashrc
```sh
$ source ~/.bashrc_ecd
```
2. restart your terminal session

### Usage
For any working directory, using following command to push it into list
```sh
$ ecd .
```
Whenever your want to jump a recorded directory, get the idx for jumping first
```sh
$ ecd -l
```

And you can jump to the directory by
```sh
$ ecd -Number, e.g. ecd -1
```

Here is the example of result from ecd -l command
```sh
0)/Volumes/Local_Data/21455305/LINUX/android
1)/Volumes/Local_Data/2144/al_Data/21455305/LINUX/android/hardware/qcom/camera/QCamera2
2)/Volumes/s/Local_Data/21455305/LINUX/android/hardware/qcom/display/libhwcomposer
3)/Volumes/Local_Data/21455305/LINUX/android/packages/apps/SnapdragonCamera
4)/Volumes/Local_Data/21455305/LINUX/android/vendor/qcom/proprietary/mm-camera/mm-camera2
```
