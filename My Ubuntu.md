# My Ubuntu

## Github Setup

Follow this [link](https://blog.csdn.net/weixin_43569276/article/details/94587416?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522171814465516800180649143%2522%252C%2522scm%2522%253A%252220140713.130102334..%2522%257D&request_id=171814465516800180649143&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~sobaiduend~default-4-94587416-null-null.142^v100^pc_search_result_base5&utm_term=ubuntu%20github%20%E9%85%8D%E7%BD%AE&spm=1018.2226.3001.4187)

## Network Setup

```
cd Documents/
git clone git@github.com:openhacker/backport_iwlwifi.git
cd backport_iwlwifi
sudo make defconfig-wilwifi-public
sudo make
sudo make install
reboot
```

## Nvidia Driver Setup

1. Remove previous driver

	```
	sudo apt-get remove --purge nvidia*
	```
2. Stop nouveau

	```
	sudo vi /etc/modprobe.d/blacklist-nouveau.conf
	
	```
	Add the following lines:
	
	```
	blacklist nouveau
	options nouveau modeset=0
	```
	Execute the change
	
	```
	sudo update-initramfs -u
	```
3. Install the driver in 

	```Software & Updates```
	
	```-> Additional Drivers```
	
	```-> Using NVIDIA driver metapackage from nvidia-driver-535 (proprietary)```

## Install VSCode
Follow this [link](https://code.visualstudio.com/docs/setup/linux)
## Install Google Chrome
Follow this [link](https://www.omgubuntu.co.uk/how-to-install-google-chrome-on-ubuntu)
## Install Google Pinyin
Follow this [link](https://blog.csdn.net/qq_44940689/article/details/132686143?ops_request_misc=&request_id=&biz_id=102&utm_term=ubuntu%20%E5%AE%89%E8%A3%85%E8%B0%B7%E6%AD%8C%E8%BE%93%E5%85%A5%E6%B3%95&utm_medium=distribute.pc_search_result.none-task-blog-2~all~sobaiduweb~default-3-132686143.142^v100^pc_search_result_base5&spm=1018.2226.3001.4187)

## Install ROS Noetic

Follow this [link](Ubuntu&ROS)