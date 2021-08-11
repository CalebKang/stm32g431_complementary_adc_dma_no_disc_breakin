# stm32g431_complementary_adc_dma_no_disc_breakin

ADC Multi trigger – Discontinuous mode disable

 1) 2 Channel Scan 
 
 2) DMA_CNDTRx 의 길이를 4로 변경
 
 3) Trigger2 이후 ADC Conversion 완료 시 Transfer Complete Callback IRQ 발생

 4) CC interrupt test while break in to TIM8

 5) TIM 동작중에 MMS 변경이 가능한지 테스트
 
 * MMS Note: The clock of the slave timer or ADC must be enabled prior to receive events from the master timer, and must not be changed on-the-fly while triggers are received from the master timer.
 
 

