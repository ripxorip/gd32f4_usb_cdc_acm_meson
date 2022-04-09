 project('gd32f4_usb_cdc_acm', 'c',
  version : '1.0',
  default_options : [
    'buildtype=plain',
    'b_asneeded=false',
    'b_pch=false',
    'b_staticpic=false',
    ],
  meson_version : '>=0.51.0')

src = [
  './src/app.c',
  './src/cdc_acm_core.c',
  './src/gd32f4xx_it.c',
  './src/usb_delay.c',
  './src/system_gd32f4xx.c',
  './contrib/GD32F4xx_Firmware_Library/Utilities/gd32f450i_eval.c',
  './contrib/GD32F4xx_Firmware_Library/Firmware/GD32F4xx_standard_peripheral/Source/gd32f4xx_exti.c',
  './contrib/GD32F4xx_Firmware_Library/Firmware/GD32F4xx_standard_peripheral/Source/gd32f4xx_gpio.c',
  './contrib/GD32F4xx_Firmware_Library/Firmware/GD32F4xx_standard_peripheral/Source/gd32f4xx_misc.c',
  './contrib/GD32F4xx_Firmware_Library/Firmware/GD32F4xx_standard_peripheral/Source/gd32f4xx_pmu.c',
  './contrib/GD32F4xx_Firmware_Library/Firmware/GD32F4xx_standard_peripheral/Source/gd32f4xx_rcu.c',
  './contrib/GD32F4xx_Firmware_Library/Firmware/GD32F4xx_standard_peripheral/Source/gd32f4xx_syscfg.c',
  './contrib/GD32F4xx_Firmware_Library/Firmware/GD32F4xx_standard_peripheral/Source/gd32f4xx_timer.c',
  './contrib/GD32F4xx_Firmware_Library/Firmware/GD32F4xx_standard_peripheral/Source/gd32f4xx_usart.c',
  './contrib/GD32F4xx_Firmware_Library/Firmware/GD32F4xx_usb_driver/Source/usb_core.c',
  './contrib/GD32F4xx_Firmware_Library/Firmware/GD32F4xx_usb_driver/Source/usbd_core.c',
  './contrib/GD32F4xx_Firmware_Library/Firmware/GD32F4xx_usb_driver/Source/usbd_int.c',
  './contrib/GD32F4xx_Firmware_Library/Firmware/GD32F4xx_usb_driver/Source/usbd_std.c',
  ]

inc = [
  './inc',
  './contrib/GD32F4xx_Firmware_Library/Firmware/CMSIS/GD/GD32F4xx/Include',
  './contrib/GD32F4xx_Firmware_Library/Firmware/GD32F4xx_standard_peripheral/Include',
  './contrib/GD32F4xx_Firmware_Library/Firmware/GD32F4xx_usb_driver/Include',
  './contrib/GD32F4xx_Firmware_Library/Utilities',
  './contrib/GD32F4xx_Firmware_Library/Firmware/CMSIS',
  './contrib/GD32F4xx_Firmware_Library/Firmware/GD32F4xx_usb_driver/Include',
]

link_args = []

exe = executable('gd32f4_usb_cdc_acm',
  [src],
  name_suffix: 'elf',
  link_args: link_args,
  include_directories : inc
)
