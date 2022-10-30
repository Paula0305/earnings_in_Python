Project description

This program was written for the programming class. It is intended to calculate the low and high rates for python developers.
The data on the basis of which we calculate the average rates comes from "http://justjoin.it/api/offers". Using the Requests library, we refer to the data we are interested in and download it in order to perform the calculations.
The first step I took was to create a "for" loop, which selected only Python programming offers for me. Then, referring to the type of employment under the ['type'] link, I divided the offers into "b2b" and "permanent". The sums of the downloaded values were saved in four variables, two for each type. For b2b offers, the highest in the variable - highest_b2b, and lowest - lowest_b2b. Correspondingly, for fixed offers, the highest in the variable - highest_per, and the lowest - lowest_per.
I also created a function that multiplies the salary by the appropriate conversion factor so that it is given in PLN. We refer to the value contained in the glossary under the reference ['salary'] ['currency'].

Finally, we divide the sums by the amount of the given offer and give rounded up to 2 decimal places.
