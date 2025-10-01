# Pulsed-LikeSignal-Generator
This project contain the app to generate Sinc, Gauss and Chirp signal with different levels of Gaussian random noise, filter deformation and ESSC parameter extraction 
generating two type of data files, one with ESSC parameters extracted from the signal and the other with raw signal samples (amplitude and time).

<figure>
  <p align="center">
  <img src="./Images/main_app_block.jpg" width="500">
  </p>
</figure>
<p align="center">
	Signal and deformed signal by GaussBurn filter type deformation.
</p>     

## Installation
In Matlab, go to `Apps Tab` and then `Install App` search for `SSC Pulso RMN - GN - DL` file and open it.

### How to use it:

Ones the app was installed, find it in APPS tab and open it.
For more detailed information have a look to **DataGenerator_Man.pdf** included in project.

1. **First Window: "Genera Señal"**  
   - A window named `Genera Señal` will be open. Select the type of pulsed-like singal to generate and the push `Genera Entrada`
   - Push `Detecta Pulso`, then `Genera Derivada` and `Genera Integral`, derivate and integral from original signal will be plot.
   - Then push `Calcula SSC` to extract 30 ESSC parameters, `Radio de Detección de Extremos` allows to set the radio which maxium or minimun
   will be detected.
   - Push `Enviar` to open a second window.
   
<figure>
  <p align="center">
  <img src="./Images/first_window.jpg" width="500">
  </p>
</figure>
<p align="center">
	First Window to generate an Ideal Signal and extrema detection - In this case Sinc pulsed signal type.
</p>   
   
 2. **Second Window: "Señal Real" (Real Signal)**  
   - A window named `Señal Real` will be open. In this case, more configuration related with Noise, Filter Deformation and Filtering is avaible.
   - Push `Detecta Pulso`, then `Genera Derivada` and `Genera Integral`, derivate and integral from original signal will be plot.
   - Then push `Calcula SSC` to extract 30 ESSC parameters, `Radio de Detección de Extremos` allows to set the radio which maxium or minimun
   will be detected.  
   - Noise, deformation filter, pulse detection ... is well explained in paper secction `3.3 Dataset Generation for ANN training`.
   - Finally push `Ejecuta Ciclo`, and two .txt files will be generated, one with 1000 raw of ESSC parameter (for Machine Learning training) and a second one with 
   amplitude and time raw data (to be use in Deep Learning training).
   
<figure>
  <p align="center">
  <img src="./Images/second_window.jpg" width="500">
  </p>
</figure>
<p align="center">
	Second Window to generate a Real Signal and extrema detection - In this case Sinc pulsed signal type.
</p>   
      
<figure>
  <p align="center">
  <img src="./Images/spectral_window.jpg" width="500">
  </p>
</figure>
<p align="center">
	Signal and deformed signal spectrum deformed by GaussBurn filter.
</p>     



## Author

- Guillermo H. Bustos 	(ghernanbustos@gmail.com)
- Héctor H. Segnorile 	(segnoh@gmail.com)
- **Institution**: Instituto de Física Enrique Gaviola (IFEG CONICET)- Universidad Nacional de Córdoba - FAMAF

