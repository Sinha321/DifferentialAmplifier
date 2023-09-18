# DifferentialAmplifier
#### A differential amplifier is a circuit whose output voltage is directly proportional to the difference between voltages applied at it's to inputs.
## The four differential amplifier configurations are following:
* Dual input, balanced output differential amplifier.
* Dual input, unbalanced output differential amplifier.
* Single input balanced output differential amplifier.
* Single input unbalanced output differential amplifier.

### Active Load Configurations for Differential Amplifiers:
1. Current mirror load
2. Current source load
3. Diode Connected Load

##### The current mirror load provides double-ended to single-ended conversion without suffering the loss of a factor of two in differential-mode gain (the common-mode gain is twice as large also, but still very small).It comes in a variety of versions (pnp, npn, nMOS, p-MOS); the examples below use p-channel MOSFETs in the mirror loading an nchannel common-source differential gain stage. 
* The active nature of the load doubles the current delivered to the load with differential-mode inputs, and while not sending any current to the load with common-mode inputs.

* Difference-mode inputs:
  
  ![DA1](https://github.com/Sinha321/DifferentialAmplifier/assets/116704941/0abbd39a-3363-44b6-8b23-4e7a179d29c0)

* Common-mode inputs:
  
  ![DA2](https://github.com/Sinha321/DifferentialAmplifier/assets/116704941/2042a0aa-4c96-4722-9e8c-378526bc0061)

#### Procedure
  * Apply DC biasing @VG1-2 = 2.5V to the gate of M1-2 and superimpose sinusoidal inputs Vin1 of 10mVp-p @1KHz and Vin2 of -10mVp-p @1KHz.
  * Also apply DC biasing VG3 = 1.4V to the gate of M5 and Vg4 = 3.6V to the gates of M3 and M4
  * Using .op statement ,note down the value of ID1-2,VGS1-2,VDS1-2,VSG3-4,VSD3-4 etc
  * Comment .op statement and use tran statement to plot Vid(t)=Vin1(t) - Vin2(t) and Vout(t)
  * Use .meas statement to note down Vidp-p, Voutp-p and voltage gain 

#### Schematic

![lt1](https://github.com/Sinha321/DifferentialAmplifier/assets/116704941/5eec790c-3ea9-4de6-9b2a-fb9be108dd1b)

#### Calculations 
* ID1=1/2 * (un * Co * W/L)(VGS1-Vth1)^2 (1+lambda1 * VDS1)
* |ID3|=1/2 * (up * Co * W/L)(VGS3-|Vth3|)^2 (1+lambda3 * VSD3)
* gm1= 2ID1/(VGS1-Vth1)
* ro1= (1+lambda1 * VDS1)/(lambda1 * ID1)
* ro3= (1+lambda3 * VDS3)/(lambda3 * ID3)

  Verify the gain by the formula
  * Av= -gmn(roN || roP)

#### Waveform
* Differential input and Differential output

  ![lt2](https://github.com/Sinha321/DifferentialAmplifier/assets/116704941/2b50ef58-bdc7-4237-943f-76181c713cfb)

  
### Applications of Differential Amplifiers
#### Generally, we use differential amplifier that acts as a volume control circuit. The differential operational amplifier can be used as an automatic gain control circuit. Some of the differential operational amplifier can be used for Amplitude modulation.
#### Differential amplifiers provide increase noise immunity: When using differential amplifiers, it responds to the only difference signal between input terminals and also ignores all common-mode signals such as noise pick–up and the ground voltage.
    

