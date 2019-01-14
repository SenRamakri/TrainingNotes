# TrainingNotes

Presentation: https://armh-my.sharepoint.com/:p:/g/personal/senthil_ramakrishnan_arm_com/EW-_omcQPHxAr2J5FBcxJf0BKAxy7taT91HYWXKSBLVtcQ?e=T6vQoP

Fault Handler Demo
==================
git clone https://github.com/ARMmbed/mbed-os-example-fault-handler

cd mbed-os-example-fault-handler

mbed deploy

mbed compile -t GCC_ARM -m K64F

__Running the parser__ :

crash_log_parser <CRASH_LOG> <PATH_TO_ELF_FILE>  <PATH_TO_MAP_FILE>

Crash Reporting Demo
==================
git clone https://github.com/ARMmbed/mbed-os-example-crash-reporting

cd mbed-os-example-crash-reporting

mbed deploy

mbed compile -t GCC_ARM -m K64F


