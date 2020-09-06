# about-tencent
    How to tailor Tencentos.
        1.首先下载内核文件中12个，选中kernel\arch \osal,把一些相关文件加到keil中，然后添加相应头文件。2 .在系统中断函数stm32l4xx_it.c中把pendsv_Handler(void)
    文件屏蔽和systick_Handler(void)函数做对应改造。3.主函数中添加相应头文件cmsis_os.h和tos_k.h，若没有添加，会编译不过去的！在配置文件tos_config.h中，加上对应开发芯片的头文件，
    如stm32l4xx.h.
    
