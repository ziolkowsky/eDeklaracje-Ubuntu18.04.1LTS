# Instalacja aplikacji  e-Deklaracje w systemie Ubuntu 18.04.1 LTS x64 


## Krok 1: Pobieranie i instalacja pakietu Adobe Air
### Polecenie:
```
wget -O adobe-air_amd64.deb http://drive.noobslab.com/data/apps/AdobeAir/adobeair_2.6.0.2_amd64.deb
```
```
 sudo dpkg -i adobe-air_amd64.deb
```
```
Selecting previously unselected package adobeair.
      (Reading database ... 182067 files and directories currently installed.)
      Preparing to unpack adobe-air_amd64.deb ...
      Unpacking adobeair (1:2.6.0.2) ...
      dpkg: dependency problems prevent configuration of adobeair:
       adobeair depends on libbz2-1.0:i386.
       adobeair depends on libc6:i386.
       adobeair depends on libgtk2.0-0:i386 (>= 2.6).
       adobeair depends on libnss3:i386.
       adobeair depends on libstdc++6:i386.
       adobeair depends on libxml2:i386.
       adobeair depends on libxaw7:i386.
       adobeair depends on libxslt1.1:i386. 
```
  [Command] sudo apt-get install libbz2-1.0:i386 -y
    [Problem] Output: 
      Selecting previously unselected package adobeair.
      Reading package lists... Done
      Building dependency tree       
      Reading state information... Done
      You might want to run 'apt --fix-broken install' to correct these.
      The following packages have unmet dependencies:
       adobeair : Depends: libc6:i386
         Depends: libgtk2.0-0:i386 (>= 2.6)
         Depends: libnss3:i386
         Depends: libstdc++6:i386
         Depends: libxml2:i386
         Depends: libxaw7:i386
         Depends: libxslt1.1:i386
       libbz2-1.0:i386 : Depends: libc6:i386 (>= 2.4) but it is not going to be installed
      E: Unmet dependencies. Try 'apt --fix-broken install' with no packages (or specify a solution).
  [Command] sudo apt-get install libbz2-1.0:i386 libc6:i386 libgtk2.0-0:i386 libnss3:i386 libstdc++6:i386 libxml2:i386 libxaw7:i386 libxslt1.1:i386
    [Problem] Output:
      Reading package lists... Done
      Building dependency tree       
      Reading state information... Done
      You might want to run 'apt --fix-broken install' to correct these.
      The following packages have unmet dependencies:
       libc6:i386 : Depends: libgcc1:i386 but it is not going to be installed
       libgtk2.0-0:i386 : Depends: libatk1.0-0:i386 (>= 1.32.0) but it is not going to be installed
                    Depends: libcairo2:i386 (>= 1.6.4-6.1) but it is not going to be installed
                    Depends: libcups2:i386 (>= 1.6.2) but it is not going to be installed
                    Depends: libfontconfig1:i386 (>= 2.12) but it is not going to be installed
                    Depends: libgdk-pixbuf2.0-0:i386 (>= 2.22.0) but it is not going to be installed
                    Depends: libglib2.0-0:i386 (>= 2.41.1) but it is not going to be installed
                    Depends: libpango-1.0-0:i386 (>= 1.28.3) but it is not going to be installed
                    Depends: libpangocairo-1.0-0:i386 (>= 1.28.3) but it is not going to be installed
                    Depends: libpangoft2-1.0-0:i386 (>= 1.28.3) but it is not going to be installed
                    Depends: libx11-6:i386 (>= 2:1.4.99.1) but it is not going to be installed
                    Depends: libxcomposite1:i386 (>= 1:0.3-1) but it is not going to be installed
                    Depends: libxcursor1:i386 (> 1.1.2) but it is not going to be installed
                    Depends: libxdamage1:i386 (>= 1:1.1) but it is not going to be installed
                    Depends: libxext6:i386 but it is not going to be installed
                    Depends: libxfixes3:i386 but it is not going to be installed
                    Depends: libxi6:i386 but it is not going to be installed
                    Depends: libxinerama1:i386 but it is not going to be installed
                    Depends: libxrandr2:i386 (>= 2:1.5.0) but it is not going to be installed
                    Depends: libxrender1:i386 but it is not going to be installed
                    Recommends: libgail-common:i386 but it is not going to be installed
       libnss3:i386 : Depends: libnspr4:i386 (>= 2:4.12) but it is not going to be installed
                Depends: libsqlite3-0:i386 (>= 3.5.9) but it is not going to be installed
       libstdc++6:i386 : Depends: gcc-8-base:i386 (= 8.2.0-1ubuntu2~18.04) but it is not going to be installed
                   Depends: libgcc1:i386 (>= 1:4.2) but it is not going to be installed
       libxaw7:i386 : Depends: libx11-6:i386 but it is not going to be installed
                Depends: libxext6:i386 but it is not going to be installed
                Depends: libxmu6:i386 but it is not going to be installed
                Depends: libxpm4:i386 but it is not going to be installed
                Depends: libxt6:i386 but it is not going to be installed
       libxml2:i386 : Depends: libicu60:i386 (>= 60.1-1~) but it is not going to be installed
                Depends: liblzma5:i386 (>= 5.1.1alpha+20120614) but it is not going to be installed
                Depends: zlib1g:i386 (>= 1:1.2.3.3) but it is not going to be installed
       libxslt1.1:i386 : Depends: libgcrypt20:i386 (>= 1.7.0) but it is not going to be installed
      E: Unmet dependencies. Try 'apt --fix-broken install' with no packages (or specify a solution).
  [Command] sudo apt-get install libbz2-1.0:i386 libc6:i386 libgtk2.0-0:i386 libnss3:i386 libstdc++6:i386 libxml2:i386 libxaw7:i386 libxslt1.1:i386 libatk1.0-0:i386 libcairo2:i386 libgcc1:i386 libcups2:i386 libfontconfig1:i386 libgdk-pixbuf2.0-0:i386 libglib2.0-0:i386 libpango-1.0-0:i386 libpangocairo-1.0-0:i386 libpangoft2-1.0-0:i386 libx11-6:i386 libxcomposite1:i386 libxcursor1:i386 libxdamage1:i386 libxext6:i386 libxfixes3:i386 libxi6:i386 libxinerama1:i386 libxrandr2:i386 libxrender1:i386 libgail-common:i386 libnspr4:i386 libsqlite3-0:i386 gcc-8-base:i386 libgcc1:i386 libx11-6:i386 libxext6:i386 libxmu6:i386 libxpm4:i386 libxt6:i386 libicu60:i386 liblzma5:i386 zlib1g:i386 libgcrypt20:i386 

    [Problem] Output: 
      Reading package lists... Done
Building dependency tree       
Reading state information... Done
You might want to run 'apt --fix-broken install' to correct these.
The following packages have unmet dependencies:
 libcairo2:i386 : Depends: libfreetype6:i386 (>= 2.7.1) but it is not going to be installed
                  Depends: libpixman-1-0:i386 (>= 0.30.0) but it is not going to be installed
                  Depends: libpng16-16:i386 (>= 1.6.2-1) but it is not going to be installed
                  Depends: libxcb-render0:i386 but it is not going to be installed
                  Depends: libxcb-shm0:i386 but it is not going to be installed
                  Depends: libxcb1:i386 (>= 1.6) but it is not going to be installed
 libcups2:i386 : Depends: libavahi-client3:i386 (>= 0.6.16) but it is not going to be installed
                 Depends: libavahi-common3:i386 (>= 0.6.16) but it is not going to be installed
                 Depends: libgnutls30:i386 (>= 3.5.6) but it is not going to be installed
                 Depends: libgssapi-krb5-2:i386 (>= 1.14+dfsg) but it is not going to be installed
 libfontconfig1:i386 : Depends: libexpat1:i386 (>= 2.0.1) but it is not going to be installed
                       Depends: libfreetype6:i386 (>= 2.2.1) but it is not going to be installed
 libgail-common:i386 : Depends: libgail18:i386 (= 2.24.32-1ubuntu1) but it is not going to be installed
 libgcrypt20:i386 : Depends: libgpg-error0:i386 (>= 1.25) but it is not going to be installed
 libgdk-pixbuf2.0-0:i386 : Depends: libjpeg8:i386 (>= 8c) but it is not going to be installed
                           Depends: libpng16-16:i386 (>= 1.6.2-1) but it is not going to be installed
                           Depends: libtiff5:i386 (>= 4.0.3) but it is not going to be installed
 libglib2.0-0:i386 : Depends: libffi6:i386 (>= 3.0.4) but it is not going to be installed
                     Depends: libmount1:i386 (>= 2.19.1) but it is not going to be installed
                     Depends: libpcre3:i386 but it is not going to be installed
                     Depends: libselinux1:i386 (>= 1.32) but it is not going to be installed
 libpango-1.0-0:i386 : Depends: libthai0:i386 (>= 0.1.22-3~) but it is not going to be installed
 libpangocairo-1.0-0:i386 : Depends: libfreetype6:i386 (>= 2.2.1) but it is not going to be installed
 libpangoft2-1.0-0:i386 : Depends: libfreetype6:i386 (>= 2.3.5) but it is not going to be installed
                          Depends: libharfbuzz0b:i386 (>= 1.2.6) but it is not going to be installed
 libx11-6:i386 : Depends: libxcb1:i386 (>= 1.11.1) but it is not going to be installed
 libxt6:i386 : Depends: libice6:i386 (>= 1:1.0.0) but it is not going to be installed
               Depends: libsm6:i386 but it is not going to be installed
E: Unmet dependencies. Try 'apt --fix-broken install' with no packages (or specify a solution).

[Command]
  sudo apt-get install libbz2-1.0:i386 libc6:i386 libgtk2.0-0:i386 libnss3:i386 libstdc++6:i386 libxml2:i386 libxaw7:i386 libxslt1.1:i386 libatk1.0-0:i386 libcairo2:i386 libgcc1:i386 libcups2:i386 libfontconfig1:i386 libgdk-pixbuf2.0-0:i386 libglib2.0-0:i386 libpango-1.0-0:i386 libpangocairo-1.0-0:i386 libpangoft2-1.0-0:i386 libx11-6:i386 libxcomposite1:i386 libxcursor1:i386 libxdamage1:i386 libxext6:i386 libxfixes3:i386 libxi6:i386 libxinerama1:i386 libxrandr2:i386 libxrender1:i386 libgail-common:i386 libnspr4:i386 libsqlite3-0:i386 gcc-8-base:i386 libgcc1:i386 libx11-6:i386 libxext6:i386 libxmu6:i386 libxpm4:i386 libxt6:i386 libicu60:i386 liblzma5:i386 zlib1g:i386 libgcrypt20:i386 libfreetype6:i386 libpixman-1-0:i386 libpng16-16:i386 libxcb-render0:i386 libxcb-shm0:i386 libxcb1:i386 libavahi-client3:i386 libavahi-common3:i386 libgnutls30:i386 libgssapi-krb5-2:i386 libexpat1:i386 libgail18:i386 libgpg-error0:i386 libjpeg8:i386 libtiff5:i386 libffi6:i386 libmount1:i386 libpcre3:i386 libselinux1:i386 libthai0:i386 libharfbuzz0b:i386 libxau6:i386 libxdmcp6:i386 libice6:i386 libsm6:i386
[Problem] Output:
Reading package lists... Done
Building dependency tree       
Reading state information... Done
You might want to run 'apt --fix-broken install' to correct these.
The following packages have unmet dependencies:
 libavahi-client3:i386 : Depends: libdbus-1-3:i386 (>= 1.9.14) but it is not going to be installed
 libavahi-common3:i386 : Depends: libavahi-common-data:i386 but it is not going to be installed
 libgnutls30:i386 : Depends: libgmp10:i386 (>= 2:6) but it is not going to be installed
                    Depends: libhogweed4:i386 but it is not going to be installed
                    Depends: libidn2-0:i386 (>= 0.6) but it is not going to be installed
                    Depends: libnettle6:i386 but it is not going to be installed
                    Depends: libp11-kit0:i386 (>= 0.23.1) but it is not going to be installed
                    Depends: libtasn1-6:i386 (>= 4.12) but it is not going to be installed
                    Depends: libunistring2:i386 (>= 0.9.7) but it is not going to be installed
 libgssapi-krb5-2:i386 : Depends: libcomerr2:i386 (>= 1.34)
                         Depends: libk5crypto3:i386 (>= 1.16) but it is not going to be installed
                         Depends: libkrb5-3:i386 (= 1.16-2build1) but it is not going to be installed
                         Depends: libkrb5support0:i386 (>= 1.15~beta1) but it is not going to be installed
 libharfbuzz0b:i386 : Depends: libgraphite2-3:i386 (>= 1.2.2) but it is not going to be installed
 libice6:i386 : Depends: libbsd0:i386 (>= 0.2.0) but it is not going to be installed
 libjpeg8:i386 : Depends: libjpeg-turbo8:i386 (>= 1.1.90+svn722-1ubuntu6) but it is not going to be installed
 libmount1:i386 : Depends: libblkid1:i386 (>= 2.17.2) but it is not going to be installed
 libsm6:i386 : Depends: libuuid1:i386 (>= 2.16) but it is not going to be installed
 libthai0:i386 : Depends: libdatrie1:i386 (>= 0.2.0) but it is not going to be installed
 libtiff5:i386 : Depends: libjbig0:i386 (>= 2.0) but it is not going to be installed
 libxdmcp6:i386 : Depends: libbsd0:i386 (>= 0.2.0) but it is not going to be installed
E: Unmet dependencies. Try 'apt --fix-broken install' with no packages (or specify a solution).

[Command] sudo apt-get install libbz2-1.0:i386 libc6:i386 libgtk2.0-0:i386 libnss3:i386 libstdc++6:i386 libxml2:i386 libxaw7:i386 libxslt1.1:i386 libatk1.0-0:i386 libcairo2:i386 libgcc1:i386 libcups2:i386 libfontconfig1:i386 libgdk-pixbuf2.0-0:i386 libglib2.0-0:i386 libpango-1.0-0:i386 libpangocairo-1.0-0:i386 libpangoft2-1.0-0:i386 libx11-6:i386 libxcomposite1:i386 libxcursor1:i386 libxdamage1:i386 libxext6:i386 libxfixes3:i386 libxi6:i386 libxinerama1:i386 libxrandr2:i386 libxrender1:i386 libgail-common:i386 libnspr4:i386 libsqlite3-0:i386 gcc-8-base:i386 libgcc1:i386 libx11-6:i386 libxext6:i386 libxmu6:i386 libxpm4:i386 libxt6:i386 libicu60:i386 liblzma5:i386 zlib1g:i386 libgcrypt20:i386 libfreetype6:i386 libpixman-1-0:i386 libpng16-16:i386 libxcb-render0:i386 libxcb-shm0:i386 libxcb1:i386 libavahi-client3:i386 libavahi-common3:i386 libgnutls30:i386 libgssapi-krb5-2:i386 libexpat1:i386 libgail18:i386 libgpg-error0:i386 libjpeg8:i386 libtiff5:i386 libffi6:i386 libmount1:i386 libpcre3:i386 libselinux1:i386 libthai0:i386 libharfbuzz0b:i386 libxau6:i386 libxdmcp6:i386 libice6:i386 libsm6:i386 libdbus-1-3:i386 libavahi-common-data:i386 libgmp10:i386 libhogweed4:i386 libidn2-0:i386 libnettle6:i386 libp11-kit0:i386 libtasn1-6:i386 libunistring2:i386 libcomerr2:i386 libk5crypto3:i386 libkrb5-3:i386 libkrb5support0:i386 libgraphite2-3:i386 libbsd0:i386 libjpeg-turbo8:i386 libblkid1:i386 libuuid1:i386 libdatrie1:i386 libjbig0:i386 libbsd0:i386
[Problem] Output:
Reading package lists... Done
Building dependency tree       
Reading state information... Done
You might want to run 'apt --fix-broken install' to correct these.
The following packages have unmet dependencies:
 libcomerr2:i386 : Depends: libcom-err2:i386 but it is not going to be installed
 libdbus-1-3:i386 : Depends: libsystemd0:i386 but it is not going to be installed
 libkrb5-3:i386 : Depends: libkeyutils1:i386 (>= 1.5.9) but it is not going to be installed
E: Unmet dependencies. Try 'apt --fix-broken install' with no packages (or specify a solution).

  [Command] sudo apt-get install libbz2-1.0:i386 libc6:i386 libgtk2.0-0:i386 libnss3:i386 libstdc++6:i386 libxml2:i386 libxaw7:i386 libxslt1.1:i386 libatk1.0-0:i386 libcairo2:i386 libgcc1:i386 libcups2:i386 libfontconfig1:i386 libgdk-pixbuf2.0-0:i386 libglib2.0-0:i386 libpango-1.0-0:i386 libpangocairo-1.0-0:i386 libpangoft2-1.0-0:i386 libx11-6:i386 libxcomposite1:i386 libxcursor1:i386 libxdamage1:i386 libxext6:i386 libxfixes3:i386 libxi6:i386 libxinerama1:i386 libxrandr2:i386 libxrender1:i386 libgail-common:i386 libnspr4:i386 libsqlite3-0:i386 gcc-8-base:i386 libgcc1:i386 libx11-6:i386 libxext6:i386 libxmu6:i386 libxpm4:i386 libxt6:i386 libicu60:i386 liblzma5:i386 zlib1g:i386 libgcrypt20:i386 libfreetype6:i386 libpixman-1-0:i386 libpng16-16:i386 libxcb-render0:i386 libxcb-shm0:i386 libxcb1:i386 libavahi-client3:i386 libavahi-common3:i386 libgnutls30:i386 libgssapi-krb5-2:i386 libexpat1:i386 libgail18:i386 libgpg-error0:i386 libjpeg8:i386 libtiff5:i386 libffi6:i386 libmount1:i386 libpcre3:i386 libselinux1:i386 libthai0:i386 libharfbuzz0b:i386 libxau6:i386 libxdmcp6:i386 libice6:i386 libsm6:i386 libdbus-1-3:i386 libavahi-common-data:i386 libgmp10:i386 libhogweed4:i386 libidn2-0:i386 libnettle6:i386 libp11-kit0:i386 libtasn1-6:i386 libunistring2:i386 libcomerr2:i386 libk5crypto3:i386 libkrb5-3:i386 libkrb5support0:i386 libgraphite2-3:i386 libbsd0:i386 libjpeg-turbo8:i386 libblkid1:i386 libuuid1:i386 libdatrie1:i386 libjbig0:i386 libbsd0:i386 libcom-err2:i386 libsystemd0:i386 libkeyutils1:i386
  [Problem] Output:
Reading package lists... Done
Building dependency tree       
Reading state information... Done
You might want to run 'apt --fix-broken install' to correct these.
The following packages have unmet dependencies:
 libsystemd0:i386 : PreDepends: liblz4-1:i386 (>= 0.0~r113) but it is not going to be installed
E: Unmet dependencies. Try 'apt --fix-broken install' with no packages (or specify a solution).

  [Command] sudo apt-get install libbz2-1.0:i386 libc6:i386 libgtk2.0-0:i386 libnss3:i386 libstdc++6:i386 libxml2:i386 libxaw7:i386 libxslt1.1:i386 libatk1.0-0:i386 libcairo2:i386 libgcc1:i386 libcups2:i386 libfontconfig1:i386 libgdk-pixbuf2.0-0:i386 libglib2.0-0:i386 libpango-1.0-0:i386 libpangocairo-1.0-0:i386 libpangoft2-1.0-0:i386 libx11-6:i386 libxcomposite1:i386 libxcursor1:i386 libxdamage1:i386 libxext6:i386 libxfixes3:i386 libxi6:i386 libxinerama1:i386 libxrandr2:i386 libxrender1:i386 libgail-common:i386 libnspr4:i386 libsqlite3-0:i386 gcc-8-base:i386 libgcc1:i386 libx11-6:i386 libxext6:i386 libxmu6:i386 libxpm4:i386 libxt6:i386 libicu60:i386 liblzma5:i386 zlib1g:i386 libgcrypt20:i386 libfreetype6:i386 libpixman-1-0:i386 libpng16-16:i386 libxcb-render0:i386 libxcb-shm0:i386 libxcb1:i386 libavahi-client3:i386 libavahi-common3:i386 libgnutls30:i386 libgssapi-krb5-2:i386 libexpat1:i386 libgail18:i386 libgpg-error0:i386 libjpeg8:i386 libtiff5:i386 libffi6:i386 libmount1:i386 libpcre3:i386 libselinux1:i386 libthai0:i386 libharfbuzz0b:i386 libxau6:i386 libxdmcp6:i386 libice6:i386 libsm6:i386 libdbus-1-3:i386 libavahi-common-data:i386 libgmp10:i386 libhogweed4:i386 libidn2-0:i386 libnettle6:i386 libp11-kit0:i386 libtasn1-6:i386 libunistring2:i386 libcomerr2:i386 libk5crypto3:i386 libkrb5-3:i386 libkrb5support0:i386 libgraphite2-3:i386 libbsd0:i386 libjpeg-turbo8:i386 libblkid1:i386 libuuid1:i386 libdatrie1:i386 libjbig0:i386 libbsd0:i386 libcom-err2:i386 libsystemd0:i386 libkeyutils1:i386 liblz4-1:i386

 

PRoblem with installation. Possible solution at: https://askubuntu.com/questions/913892/how-to-install-scratch-2-on-ubuntu-16-10-or-17-04-64bit
