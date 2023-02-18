# AnotherPeakCalling-ATAC
Based on an idea I had on stats class. Make a computational effcient way to call peaks on noisy ATAC-Seq data. 

## Base Idea: 
Using a slide window to compute the mean and standard deviation of each genome chunk. given that a peak usually appears (as what a human eye would tell) with the derivative being extremely high, then extremely low. A peak would be defined as a genome fragments that consist three parts: $L_1$: peak rising, $L_2$: peak plateau, and $L_3$: peak decsending. With the following charactertistics. $p = the threshold$
$$ \sigma_{L_1} \geq p; \sigma_{L_2} \approx 0; \mu_{L_2} > \mu_{all}; \sigma_{L_3} \leq -p $$

We'll see how it goes...

