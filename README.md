# Ubuntu Wifi module installation
Due to kernel update in ubuntu you are no more able to get the header file for your wifi in lwfinger rtlwifi_new repo so this repo contains code to install rtl8723de wifi module in your ubuntu laptop or pc. This works for kernel version>=5.0 as well.

Following are the steps:-

## Step 1
``sudo apt-get install build-essential dkms``

## Step 2
``git clone https://github.com/smlinux/rtl8723de.git``

## Step 3
``sudo dkms add ./rtl8723de``

## Step 4
``sudo dkms install rtl8723de/5.1.1.8_21285.20171026_COEX20170111-1414``

## Step 6
``sudo modprobe -r rtl8723de``

## Step 7
``sudo modprobe rtl8723de``


Done!!!
