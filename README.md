# driversimp
understanding

Resource:

https://docs.oracle.com/cd/E23824_01/html/819-3196/docinfo.html#scrolltoc

https://dlc.openindiana.org/docs/osol/20090715/DRIVERTUT/html/ffdqq.html

https://www.cs.dartmouth.edu/~sergey/cs108/2009/Device_Drivers_Hands_on_Lab.pdf



gcc -D_KERNEL -m64 -mcmodel=kernel -c -O name.c

ld -r -o nameDRIVER name.o (ld -dy skeleton dscel.o -N misc/<name>)


(sudo rm /usr/kernel/drv/amd64/skeleton)


sudo cp skeleton /usr/kernel/drv/amd64/

sudo cp skeleton.conf /usr/kernel/drv/


sudo add_drv skeleton

sudo rem_drv skeleton

(sudo update_drv skeleton)


'# echo ddd > /devices/pseudo/skeleton@0:skel

'# cat /devices/pseudo/skeleton@0:skel
