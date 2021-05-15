# Ryzentosh-google-drive
Repackaged installation file to prevent Google Drive from installing as the ARM version due to CPU grasp issue in Ryzentosh

## How to Use

1. Unzip downloaded Google Drive.pkg file
  	```
	mkdir Google-Drive
	cd Google-Drive
	xar -xf ../GoogleDrive.pkg
  	```
2. Replace the Distribution file in the folder with the new downloaded Distribution file
3. Repackage Google-Drive.pkg file
	```
	cd Google-Drive
	xar --compression none -cf ../GoogleDrive-AMD.pkg *
	```
