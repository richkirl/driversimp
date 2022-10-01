# driversimp
understanding

Resource:

https://docs.oracle.com/cd/E23824_01/html/819-3196/docinfo.html#scrolltoc

https://dlc.openindiana.org/docs/osol/20090715/DRIVERTUT/html/ffdqq.html

https://www.cs.dartmouth.edu/~sergey/cs108/2009/Device_Drivers_Hands_on_Lab.pdf



gcc -D_KERNEL -m64 -mcmodel=kernel -c -O name.c

ld -r -o nameDRIVER name.o (ld -dy -r -o nameDRIVER name.o -N misc/mySymbols)(1)



(sudo rm /usr/kernel/drv/amd64/skeleton)


sudo cp skeleton /usr/kernel/drv/amd64/

sudo cp skeleton.conf /usr/kernel/drv/


sudo add_drv skeleton

modinfo | grep nameDRIVER


sudo rem_drv skeleton

(sudo update_drv skeleton)


'# echo ddd > /devices/pseudo/skeleton@0:skel

'# cat /devices/pseudo/skeleton@0:skel



![Screenshot at 2022-10-01 10-15-08](https://user-images.githubusercontent.com/61930048/193404563-acf15e8a-6e54-4f8e-8bf6-666c895969b3.png)


`# add_drv -i\"pci1028,20e\" skeleton

                      ^wireless-network controller for example(2)

![Screenshot at 2022-10-01 14-41-15](https://user-images.githubusercontent.com/61930048/193414817-776f74c4-f766-4013-b204-34b5cf124ceb.png)



1

(https://docs.oracle.com/cd/E23824_01/html/821-1461/ld-1.html#REFMAN1ld-1)

(https://docs.oracle.com/cd/E23824_01/html/819-0690/chapter2-90421.html#scrolltoc)

2


prtconf -vp

![Screenshot at 2022-10-01 14-47-46](https://user-images.githubusercontent.com/61930048/193415117-fdf54c1f-999a-4c29-bcf7-b61283fc41b5.png)


