use parerllel port jtag download code in linux enviroment
need install  
/usr/include/sys/io.h 	libc0.1-dev-i386 [kfreebsd-amd64], libc6-dev-amd64 [i386], libc6-dev-i386 [amd64] 

ll@debian:/opt/github/jflash_linux/jflash_linux/Jflash$ ./Jflash-s3c2440 

+------------------------------------+
|     SEC JTAG FLASH for 2440+        
|     modified by Quasar 2003.9.22+   
+------------------------------------+
Usage: SJF <filename> /t=<flash_type> /d=<delay>
Flash Type List
  1:SMDK2440:K9S3208 4MB
  2:SMDK2440:K9S6408 8MB
  3:SMDK2440:K9S2808 16MB
  4:SMDK2440:K9S5608 32MB
  5:SMDK2440:K9S1208 64MB
  6:SMDK2440:AM29LV800BB

root@debian:/opt/s3c2440_work/tool/jtag/for_linux# ./Jflash-s3c2440 u-boot.bin  /t=5 /d=5

+------------------------------------+
|     SEC JTAG FLASH for 2440+        
|     modified by Quasar 2003.9.22+   
+------------------------------------+
> flashType=5
> S3C2440X(ID=0x0032409d) is detected.

[K9S1208 NAND Flash JTAG Programmer]
ERROR: K9S1208 is not detected. Detected ID=0xecda.

need modify the support fof ID=0xecda

