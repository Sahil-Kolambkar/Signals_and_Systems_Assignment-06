%% DTFT OF A SEQUENCE

clc;
close all;
clear all;
n = 0:1:128;
x = cos(pi*n/4);
k = -300:300;
w = (pi/128)*k;
X = x*(exp(-j*pi/128)).^(n'*k);
subplot(3,1,1);
stem(n,x)
title('Input signal')
xlabel('Time')
ylabel('Amplitude')
Xm = abs(X);
subplot(3,1,2);
plot(w/pi, Xm);
axis([-3 3 0 60]);
title('Magnitude of DTFT Signal')
xlabel('Frequecy (pi units)')
ylabel('Phase');
Xp = phase(X);
subplot(3,1,3);
plot(w/pi , Xp);
title('Phase of the DTFT signal');
xlabel('Frequency (pi units)');
ylabel('Magnitude')
