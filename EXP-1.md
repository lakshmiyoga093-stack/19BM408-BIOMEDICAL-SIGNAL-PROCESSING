# GENERATION OF STANDARD DISCRETE-TIME SIGNALS
# AIM:
To generate and plot standard discrete-time signals using MATLAB.
# APPARATUS REQUIRED:
•	Computer / Laptop
•	MATLAB software
# THEORY:
Discrete-time signals are signals defined only at integer values of time (n).
These signals are basic building blocks in Digital Signal Processing (DSP) and are used for system analysis, filtering, and signal modeling.
Standard discrete-time signals include:
	Unit Impulse
	Unit Step
	Ramp
	Exponential
	Sinusoidal
	Damped Sinusoidal
In MATLAB, discrete-time signals are represented using vectors and plotted using the stem() command.
 Standard Discrete-Time Signals
 
🔹 1. Unit Impulse Signal
δ(n)={■(1,&n=0@0,&n≠0)┤

🔹 2. Unit Step Signal
u(n)={■(1,&n≥0@0,&n<0)┤

🔹 3. Ramp Signal
r(n)=n⋅u(n)

🔹 4. Exponential Signal
x(n)=a^n

🔹 5. Sinusoidal Signal
x(n)=sin⁡(ωn)

🔹 6. Damped Sinusoidal Signal
x(n)=a^n sin⁡(ωn)

# ALGORITHM:
1.	Start the program
2.	Define the sample index n
3.	Generate each standard discrete-time signal
4.	Plot the signal using stem()
5.	Label the axes and title
6.	Stop the program

# MATLAB CODE:
% GENERATION OF STANDARD DISCRETE-TIME SIGNALS

clc;
clear;
close all;

%% Sample index
n = -10:10;

%% 1. Unit Impulse Signal
x1 = (n == 0);
figure;
stem(n, x1, 'filled');
title('Unit Impulse Signal');
xlabel('n'); ylabel('Amplitude');
grid on;

%% 2. Unit Step Signal
x2 = (n >= 0);
figure;
stem(n, x2, 'filled');
title('Unit Step Signal');
xlabel('n'); ylabel('Amplitude');
grid on;

%% 3. Ramp Signal
n1 = 0:10;
x3 = n1;
figure;
stem(n1, x3, 'filled');
title('Ramp Signal');
xlabel('n'); ylabel('Amplitude');
grid on;

%% 4. Exponential Signal
a = 0.8;
x4 = a.^n1;
figure;
stem(n1, x4, 'filled');
title('Exponential Signal');
xlabel('n'); ylabel('Amplitude');
grid on;

%% 5. Sinusoidal Signal
x5 = sin(0.3*pi*n1);
figure;
stem(n1, x5, 'filled');
title('Sinusoidal Signal');
xlabel('n'); ylabel('Amplitude');
grid on;

%% 6. Damped Sinusoidal Signal
x6 = (0.9.^n1).*sin(0.4*pi*n1);
figure;
stem(n1, x6, 'filled');
title('Damped Sinusoidal Signal');
xlabel('n'); ylabel('Amplitude');
grid on;

# OUTPUT GRAPH:
<img width="723" height="735" alt="image" src="https://github.com/user-attachments/assets/1b6995fd-bd3b-4d09-a6e3-d8f177a9ec8b" />
<img width="742" height="790" alt="image" src="https://github.com/user-attachments/assets/20d57a19-8d9d-4ff1-a59b-5af71025e9ea" />
<img width="745" height="777" alt="image" src="https://github.com/user-attachments/assets/b0ab671d-a1bb-4124-81ff-161bb871823d" />
<img width="742" height="781" alt="image" src="https://github.com/user-attachments/assets/dd7d9b84-0f95-438f-8f35-feb6a8e84a78" />
<img width="738" height="873" alt="image" src="https://github.com/user-attachments/assets/6b793881-b40d-4174-8af5-ba5aa95f06fb" />
<img width="742" height="837" alt="image" src="https://github.com/user-attachments/assets/17fe03ca-b025-4405-8bb1-fdbb08389f9b" />



# Result :
Thus, standard discrete-time signals were successfully generated and plotted using MATLAB.



