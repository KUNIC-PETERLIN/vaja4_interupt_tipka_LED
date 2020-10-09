# vaja4_interupt_tipka_LED

Za digitalni vhod kot interrupt (GPIO_EXT…) uporabimo pin <b>PA0 (GPIO:EXTl)0</b>

Naslov izhodnih pinov za zeleno in modro LED: <b>PC9 in PC8</b>

Ukaz za vklop/izklop zelene LED <b>HAL_GPIO_TogglePin(LD3_GPIO_Port, GPIO_PIN_9);</b>

Ukaz za utripanje modre LED: <b>HAL_GPIO_TogglePin(LD2_M_GPIO_Port, GPIO_PIN_8);</b>

Delay za pol sekunde: <b> HAL_Delay(500);</b>

Ko pritisnemo na modro tipko na STM32L1 se nam vklopi ali izklopi zelena LED dioda.

Pri pritisku na modro tipko se utripanje modre LED dioda ne spremeni.

