# Motion board

## Motor drajver
Koristimo eksterni Pololu Dual G2 motor drajver za oba motora. [Link](https://www.pololu.com/product/2515)

## Mikro kontroler
Koristimo [STM32F446RE](https://www.st.com/en/microcontrollers-microprocessors/stm32f446re.html) cip jer ima:

- 2 x 32 bit tajmera za motor enkodere (TIM2, TIM5)
- 2 x 13 bit tajmera za odom enkodere (TIM3, TIM4)
- dovoljno tajmera za pwm (TIM1)
- CAN interface (CAN 2.0)

Moze se kupiti preko digikey [link](https://www.digikey.com/en/products/detail/stmicroelectronics/STM32F446RET6/5175962)

Ima i svoj [nucleo board](https://elektroleum.rs/product/razvojna-ploca-stmicroelectronics-nucleo-f446re/) 


## Wiring
(TIM3) PA6 - ENC1_A

(TIM3) PA7 - ENC1_B

(TIM4) PB6 - ENC2_A

(TIM4) PB7 - ENC2_B

(CAN2_TX) - PB13
(CAN2_RX) - PB12 

## TODO
- [] Dodati arduino uno headere za pololu shield
- [] Dodati CAN komunikaciju
- [] Videti koje motor enkoder konektore imamo
- [] Izdvojiti pinove za programiranje preko ST-LINK 
- [] Dodati dugme za reset
- [] Dodati lampice na can-u
- [] Dodati IMU
- [] Dodati lampice na st link
- [] ...
