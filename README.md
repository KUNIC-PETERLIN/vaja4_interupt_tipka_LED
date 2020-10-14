# vaja4_interupt_tipka_LED

Za digitalni vhod kot interrupt (GPIO_EXT…) uporabimo pin <b>PA0 (GPIO:EXTl)</b>

Naslov izhodnih pinov za zeleno in modro LED: <b>PC9 in PC8</b>

Ukaz za vklop/izklop zelene LED <b>HAL_GPIO_TogglePin(LD3_GPIO_Port, GPIO_PIN_9);</b>

Zakasnitev, ki je bila navedena je <b>10000ms</b>, a je za tipko bolj ustrezna zaksnitev <b>6000ms</b>

Ukaz za utripanje modre LED: <b>HAL_GPIO_TogglePin(LD2_M_GPIO_Port, GPIO_PIN_8);</b>

Delay za pol sekunde: <b> HAL_Delay(500);</b>

Ko pritisnemo na modro tipko na STM32L1 se nam <b>vklopi ali izklopi zelena LED dioda.</b>

Pri pritisku na modro tipko se <b>  utripanje modre LED dioda ne spremeni.</b>

<pre><strong>Komentar:</strong>
Program na plaščici STM32L1 z frekvenco 2Hz (pol sekunde) prižiga modro LED dioda. Poleg tega se ob vsakem pritisku na modro tipko prižge ali ugasne zelena LED dioda. Pri tej tipki se v programu še uporabi zakasnitev "for(uint32_t i=0; i&lt;6000; i++);", ki nam omogoči bolj tekoče delovanje prižiga LED diode. 
</pre>
