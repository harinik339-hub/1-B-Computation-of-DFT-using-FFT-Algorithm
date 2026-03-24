# EXPT 1b: Computation-of-DFT-using-FFT-ALGORITHM

## AIM
To perform and verify DFT using FFT-ALGORITHM by SCILAB.
## APPARATUS REQUIRED
PC installed with SCILAB
## PROGRAM 
### DFT FFT-ALGORITHM
```
clc;
clear;
close;
xn=[1 2 3 1 1 2 0 0];
n1=0:1:length(xn)-1;
subplot(2,2,1);
plot2d3(n1,xn);
xlabel('time n');
ylabel('amplitude');
title('input sequence');
xk=fft(xn);
k1=0:1:length(xk)-1;
magnitude=abs(xk)
subplot(2,2,2);
plot2d3(k1,magnitude);
xlabel('frequency(Hz)');
ylabel('magnitude(gain)');
title('magnitude spectrum');
angle=atan(imag(xk),real(xk));
subplot(2,2,3);
plot2d3(k1,angle);
xlabel('frequency(Hz)');
ylabel('Phase');
title('phase spectrum');
y=ifft(xk);
n2=0:1:length(y)-1;
subplot(2,2,4);
plot2d3(n2,y);
xlabel('time n');
ylabel('amplitude');
title('inverse FFT of x(k)');
disp(xk);
```
<br>
### CALCULATIONS:

![WhatsApp Image 2026-03-24 at 10 06 40 PM](https://github.com/user-attachments/assets/be1e440e-ef1e-4417-9592-188c89464004)

![WhatsApp Image 2026-03-24 at 10 06 40 PM (1)](https://github.com/user-attachments/assets/95a4337f-e02b-4135-a130-fdda99c384d5)

![WhatsApp Image 2026-03-24 at 10 06 39 PM](https://github.com/user-attachments/assets/47032be8-549b-4c7e-991d-9c7494776800)



### SAMPLE OUTPUT:
<img width="1236" height="843" alt="image" src="https://github.com/user-attachments/assets/131f2270-f79e-4b30-a687-379984ad5558" />



## RESULT:
Thus,  DFT using FFT-ALGORITHM for two given sequences were performed and its result was verified.

