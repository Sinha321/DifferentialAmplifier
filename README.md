# DifferentialAmplifier
#### A differential amplifier is a circuit whose output voltage is directly proportional to the difference between voltages applied at it's to inputs.
## The four differential amplifier configurations are following:
* Dual input, balanced output differential amplifier.
* Dual input, unbalanced output differential amplifier.
* Single input balanced output differential amplifier.
* Single input unbalanced output differential amplifier.

### Two Active Loads for Differential Amplifiers:
1. Current mirror load
2. Lee load

##### The current mirror load provides double-ended to single-ended conversion without suffering the loss of a factor of two in differential-mode gain (the common-mode gain is twice as large also, but still very small).It comes in a variety of versions (pnp, npn, nMOS, p-MOS); the examples below use p-channel MOSFETs in the mirror loading an nchannel common-source differential gain stage. 
* The active nature of the load doubles the current delivered to the load with differential-mode inputs, and while not sending any current to the load with common-mode inputs.

* Difference-mode inputs:
  
  ![DA1](https://github.com/Sinha321/DifferentialAmplifier/assets/116704941/0abbd39a-3363-44b6-8b23-4e7a179d29c0)

* Common-mode inputs:
  
  ![DA2](https://github.com/Sinha321/DifferentialAmplifier/assets/116704941/2042a0aa-4c96-4722-9e8c-378526bc0061)

#### Analysis
* Vton = 0.7V   kn=60uA/V^2   lambda(n) = 0.08V-1   Ln = 5um   W1-2 = 22um  W3
* 
