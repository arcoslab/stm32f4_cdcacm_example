stm32f4_cdcacm_example
======================

CDCACM example code for the stm32f4discovery using libopencm3 and libopencm3-plus.

This example was made in order to have a nice initial working example for using the USB as a normal communication channel between the uC and a PC.

scanf and printf are used in this example. Libopencm3-plus uses usb cdcacm in interrupt mode, therefore to allow scanf and printf to execute at any point of your programs a circular buffer plus a mutex protection is used.

This example is intended to be used on a stm32f4discovery board, but modify it to use it on other stm32f4 uC shouldn't be too difficult. (Modification to libopencm3-plus may be necessary also).
