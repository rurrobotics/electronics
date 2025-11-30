# Motion board

## Motor drajver
Koristimo eksterni Pololu Dual G2 motor drajver za oba motora. [Link](https://www.pololu.com/product/2515)

## Mikro kontroler
Koristimo [STM32G474RET6](https://www.st.com/en/microcontrollers-microprocessors/stm32g474re.html) cip jer ima:

- 2 x 32 bit tajmera za motor enkodere (TIM2, TIM5)
- 2 x 13 bit tajmera za odom enkodere (TIM3, TIM4)
- dovoljno tajmera za pwm (TIM1)
- CAN interface 

Moze se kupiti preko digikey [link](https://www.digikey.com/en/products/detail/stmicroelectronics/STM32G474RET6/10326780)

Ima i svoj [nucleo board](https://www.st.com/en/evaluation-tools/nucleo-g474re.html) 


## Wiring
(TIM3) PA4 - ENC1_A

(TIM3) PA6 - ENC1_B

(TIM4) PA11 - ENC2_A

(TIM4) PA12 - ENC2_B

## TODO
- [] Dodati arduino uno headere za pololu shield
- [] Dodati CAN komunikaciju
- [] Videti koje motor enkoder konektore imamo
- [] ...
