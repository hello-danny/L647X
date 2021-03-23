### 1. Информация по драйверам L64XX
>![](/assets/images/L6470-L6472-L6474-chart.png)
*Рис.1 Группировка драйверов по ST*

>![](/assets/images/L6472-74-82-84-Current-control-difference.png)
*Рис.2 Отличия L64XX:*
*- L6470: управление по напряжению*
*- L6472: управление по току с упреждением (?)*
*- L6474: управление по току, без упреждения*

### 2. Девелоперские платы с драйверами L64XX

>![](/assets/images/Eval-Softvare-Boards-Setup.png)
Рис.3  Cуществующие девелоперские платы для L64XX

#### 2.1 Расширения для Nucleo без встроенного МК (X-NUCLEO-IHMXX)
- X-NUCLEO-IHM02A1 2хL6470, до 4 плат стопкой
- c L6472 платы расширения для Nucleo нет
- X-NUCLEO-IHM01A1 1хL6474, до 3 плат стопкой

>![](/assets/images/X-NUCLEO-IHM02A1-pic.png)
Рис. Двухдрайверная X-NUCLEO-IHM02A1 L6470

>![](/assets/images/hucleo-L647X-hats.png)
*Рис.4 Существующие платы для Nucleo на этих драйверах*

#### 2.2 Тестовые драйверные платы с МК (EVAL64XX-DISC)
- EVAL6470H-DISC c STM32F105RBT6
- EVAL6472H-DISC c STM32F105RBT6
- c L6474 тестовая плата снята с производства

>![](/assets/images/L6472-Discovery-board.png)
*Рис.5 EVAL6472H-DISC L6472H драйверная плата с STM32F105RBT6*

#### 2.3 Раздельные комплекты интерфейсной и драйверной тестовых плат (EVAL64XX и STEVAL)
- EVAL6470H/PD
- EVAL6472H/PD
- EVAL6474H/PD

>![](/assets/images/STEVAL-PCC009V2-interface-board.png)
*Рис.6 STEVAL-PCC009V2 с STM32F103RBT6 интерфейсная плата для EVAL64XX*

>![](/assets/images/EVAL6472PD-driver-board.png)
*Рис.7 EVAL6472PD драйверная плата*


### 3. Информация по МК для драйверов L64XX
>![](/assets/images/st-key-selection-mcu.png)
*Рис.8 Выбор STM по типам двигателей (как это связано?)*

>![](/assets/images/nucleo-L64XX-hats-compatibility.png)
Рис.9 Совместимость плат расширения с Nucleo

### 4. OEM код для МК
##### STM32F103RBT6
- EVAL6470H/PD + STEVAL-PCC009V2 firmware **STSW-SPIN004**
- EVAL6472H/PD + STEVAL-PCC009V2 firmware **STSW-SPIN004**
- EVAL6474H/PD + STEVAL-PCC009V2 firmware **X-CUBE-SPN1**

##### STM32 Nucleo F4, F0, L0
- X-NUCLEO-IHM02A1 2хL6470 firmware **X-CUBE-SPN2**
- X-NUCLEO-IHM01A1 1хL6474 firmware **X-CUBE-SPN1**

##### STM32F105RBT6
- EVAL6470H-DISC firmware **STSW-SPIN004**, **STSW-SPINDISC01**
- EVAL6472H-DISC firmware **STSW-SPIN004**, **STSW-SPINDISC01**
