# Training notes

Presentation: https://armh-my.sharepoint.com/:p:/g/personal/senthil_ramakrishnan_arm_com/EW-_omcQPHxAr2J5FBcxJf0BKAxy7taT91HYWXKSBLVtcQ?e=T6vQoP

Fault Handler Demo
==================
git clone https://github.com/ARMmbed/mbed-os-example-fault-handler

cd mbed-os-example-fault-handler

mbed deploy

mbed compile -t GCC_ARM -m K64F

cp .\BUILD\K64F\ARM\mbed-os-example-fault-handler.bin D:\

Reset the board and observer serial output.

Copy the serial port output into crash.txt for running the parser.

__Running the parser__ :

python crash_log_parser.py <CRASH_LOG> <PATH_TO_ELF_FILE>  <PATH_TO_MAP_FILE>

__Example__ :
python crash_log_parser.py ./crash.txt .\BUILD\K64F\ARM\mbed-os-example-fault-handler.elf .\BUILD\K64F\ARM\mbed-os-example-fault-handler.map

Crash Reporting Demo
====================
git clone https://github.com/ARMmbed/mbed-os-example-crash-reporting

cd mbed-os-example-crash-reporting

mbed deploy

mbed compile -t GCC_ARM -m K64F

cp .\BUILD\K64F\ARM\mbed-os-example-crash-reporting.bin D:\

Reset the board and observer serial output.

Error Decoding URL
==================
https://armmbed.github.io/mbedos-error/

__Some example error codes you can try__ :
0x8001013D
0x80010125
0x8001011F



