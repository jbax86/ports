# Custom Portfiles for vcpkg

**how to get this working**

There are a few things you have to do to get a port file working in the portfile for each package you need to edit the portfile.json for a few things

1. portfile.cmake file edit sha512 to 0 for all the vcpkg_from_github listings then go to github click a commit you want it to be frozen at click browse files then find the download archive link and right click it and copy link address paste this into something and copy just the unique part it will look like __516c599636e193bad0b023379fcf157ee101869c__ save this but keep it open you need to still edit the sha512.
2. type vcpkg install package it will fail but it will say the sha 512 if setup correctly it will say the correct sha is this but your file says 0000000000000000000000000000000000000000 edit portfile.cmake and save and close it if it only has 1 download if not edit all the same way.
3. type vcpkg install package again once all the shas are fixed it will install and you should be all set.
