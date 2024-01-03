# Exp-6-Synchornous-counters - up counter and down counter 
### AIM: To implement 4 bit up and down counters and validate  functionality.
### HARDWARE REQUIRED:  – PC, Cyclone II , USB flasher
### SOFTWARE REQUIRED:   Quartus prime
### THEORY 

## UP COUNTER 
The counter is a digital sequential circuit and here it is a 4 bit counter, which simply means it can count from 0 to 15 and vice versa based upon the direction of counting (up/down). 

The counter (“count“) value will be evaluated at every positive (rising) edge of the clock (“clk“) cycle.
The Counter will be set to Zero when “reset” input is at logic high.
The counter will be loaded with “data” input when the “load” signal is at logic high. Otherwise, it will count up or down.
The counter will count up when the “up_down” signal is logic high, otherwise count down

Since we know that binary count sequences follow a pattern of octave (factor of 2) frequency division, and that J-K flip-flop multivibrators set up for the “toggle” mode are capable of performing this type of frequency division, we can envision a circuit made up of several J-K flip-flops, cascaded to produce four bits of output.
The main problem facing us is to determine how to connect these flip-flops together so that they toggle at the right times to produce the proper binary sequence.
Examine the following binary count sequence, paying attention to patterns preceding the “toggling” of a bit between 0 and 1:
Binary count sequence, paying attention to patterns preceding the “toggling” of a bit between 0 and 1.

Note that each bit in this four-bit sequence toggles when the bit before it (the bit having a lesser significance, or place-weight), toggles in a particular direction: from 1 to 0.



 
 

Starting with four J-K flip-flops connected in such a way to always be in the “toggle” mode, we need to determine how to connect the clock inputs in such a way so that each succeeding bit toggles when the bit before it transitions from 1 to 0.

The Q outputs of each flip-flop will serve as the respective binary bits of the final, four-bit count:

 
 

Four-bit “Up” Counter
![image](https://user-images.githubusercontent.com/36288975/169644758-b2f4339d-9532-40c5-af40-8f4f8c942e2c.png)



## DOWN COUNTER 

As well as counting “up” from zero and increasing or incrementing to some preset value, it is sometimes necessary to count “down” from a predetermined value to zero allowing us to produce an output that activates when the zero count or some other pre-set value is reached.

This type of counter is normally referred to as a Down Counter, (CTD). In a binary or BCD down counter, the count decreases by one for each external clock pulse from some preset value. Special dual purpose IC’s such as the TTL 74LS193 or CMOS CD4510 are 4-bit binary Up or Down counters which have an additional input pin to select either the up or down count mode.
![image](https://user-images.githubusercontent.com/36288975/169644844-1a14e123-7228-4ed8-81a9-eb937dff4ac8.png)


4-bit Count Down Counter
### Procedure
/* write all the steps invloved */



### PROGRAM 




UP COUNTER :



![UPCOUNTER CODE](https://github.com/23004345/Exp-7-Synchornous-counters-/assets/138849203/3aeafa28-cccb-4d56-bbe3-423cb424cb51)





DOWN COUNTER : 





![DOWNCOUNTER CODE](https://github.com/23004345/Exp-7-Synchornous-counters-/assets/138849203/90bb0bc1-7669-434c-a650-626cb40a8d66)




OUTPUT:





/*
Program for flipflops  and verify its truth table in quartus using Verilog programming.
Developed by: DEVESH.S
RegisterNumber:  23004345
*/






### RTL 




UP COUNTER :




![UPCOUNTER RTL](https://github.com/23004345/Exp-7-Synchornous-counters-/assets/138849203/7f1436e6-468b-4722-a6b6-6f6abec2915e)







DOWN COUNTER : 




![DOWNCOUNTER RTL](https://github.com/23004345/Exp-7-Synchornous-counters-/assets/138849203/1ffa9d66-aeae-4b3b-b450-a77f1001fe91)








### TIMING DIGRAMS FOR COUNTER  :






UP COUNTER :








![UP TIME](https://github.com/23004345/Exp-7-Synchornous-counters-/assets/138849203/fccd2ac6-0a24-476c-8088-114601f5c884)




DOWN COUNTER : 









![THE REAL DOWN TIME](https://github.com/23004345/Exp-7-Synchornous-counters-/assets/138849203/0cb80600-eba8-473b-865f-a09ab022c6e7)



### TRUTH TABLE 

UP COUNTER :







![UP TT TABLE](https://github.com/23004345/Exp-7-Synchornous-counters-/assets/138849203/a70c3cc5-35ff-4b1c-8249-97e8c75a15f7)






DOWN COUNTER : 






![DOWN TT](https://github.com/23004345/Exp-7-Synchornous-counters-/assets/138849203/9e0369bc-5cc1-4e5b-8bd8-6e5112bf517f)






### RESULTS 





Thus Synchornous counters up counter and down counter circuit are studied and the truth table for
different logic gates are verified.
