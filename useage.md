# Custom Portfiles for vcpkg

**how to get this working**

Download vcpkg and install it once thats done copy the folders in this repo into the ports folder of vcpkg repo edit details down below to freeze at your prefered commit.

To get a custom commit working you need to do a few things for each port file

1. change the ref to the ref from a commits archive.
2. change the sha512 to 0 and save keep it open cause you will replace this with real sha512 after trying to install the package.
3. after you try to install the package in the error string it will tell you the sha512 change it in the portfile and save and try again.

bgfx portfile from https://github.com/julianxhokaxhiu/FFNx and modified to work on the newest commits at the time.
