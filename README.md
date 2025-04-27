# odr_dabmux_gui

a pyhton web interface for managing odr dabmux configuration


## prerequisite

a compiled copy of odr-dabmux

## installation process

to install the gui,  
**git clone https://github.com/davidea72/odr_dabmux_gui/**


in the dir there are 2 file.  
**dabmux.service**  
**odr_dabmux_gui.service**  

this two file are the unit file for daemonize odr-dabmux and the gui in a systemd process

please copy this file under  

**/lib/systemd/system/**

followed by this command

**systemctl enable dabmux**  
**systemctl enable odr_dabmux_gui**  
**systemctl start dabmux**  
**systemctl start odr_dabmux_gui**  

to see the output from the above daemon

**journalctl -f -xeu dabmux**  
**journalctl -f -xeu odr_dabmux_gui**  

# todo

a web page to manage user  
add a selection for the protection profile A/B  

