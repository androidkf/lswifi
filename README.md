    lswifi command for Mac OS X
    ==========================
    
    This is an utility to easily list wifi SSIDS in Mac OS X, just like the `iwconfig wlan0 scan` command in Linux. It leverages the data from the `/System/Library/PrivateFrameworks/Apple80211.framework/Versions/Current/Resources/airport -s` built-in command available in Mac. You can type `lswifi` to get the unmodified output of `/System/Library/PrivateFrameworks/Apple80211.framework/Versions/Current/Resources/airport -s`.
    
    To install, clone the repository and copy to a location available in your PATH, for example `sudo cp lsusb /usr/sbin`. You can also install it with [Homebrew](http://brew.sh):
    
    ```
    brew update             && \
    brew tap jlhonora/lsusb && \
    brew install lswifi
    ```
    
    Here's an output example:
    
    ```
                              SSID BSSID             RSSI CHANNEL HT CC SECURITY (auth/unicast/group)
                          U-Mac-5G b0:26:80:9e:cb:5c -80  56      Y  CN WPA(PSK/AES/AES) WPA2(PSK/AES/AES) 
                        U-Phone-5G b0:26:80:9e:cb:5c -80  56      Y  CN WPA(PSK/AES/AES) WPA2(PSK/AES/AES) 
                           U-Guest b0:26:80:9e:cb:5c -80  56      Y  CN WPA(PSK/AES/AES) WPA2(PSK/AES/AES) 
                        U-Phone-5G b0:26:80:8e:3d:bc -57  11      Y  CN WPA(PSK/AES/AES) WPA2(PSK/AES/AES) 
                        U-Mac-2.4G b0:26:80:86:3d:b2 -57  11      Y  CN WPA(PSK/AES/AES) WPA2(PSK/AES/AES) 
 
    ```
    
    ## Usage ##
    
    ```
    lswifi
    ```
