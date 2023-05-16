# Generation-of-Discrete-Time-Signals-Using-Matlab



The unit sample sequence
In words, the unit sample sequence is a signal that is zero everywhere except at
n=0 where its value is unity. This signal is sometimes referred to as a unit
impulse.

N=13;
a=0:1:N-1;
b=[ones(1,1),zeros(1,N-1)];
subplot(3,2,1);
stem(a,b,&#39;b&#39;);
xlabel(&#39;a&#39;);
ylabel(&#39;b&#39;);
title(&#39;The Unit Sample Signal&#39;);


The unit step signal
A signal with magnitude one for time greater than zero.We can assume it as a dc
signal which got switched on at time equal to zero.

N=13;
a=0:1:N-1;
b=ones(1,N);
subplot(3,2,2);
stem(a,b,&#39;b&#39;);
xlabel(&#39;a&#39;);
ylabel(&#39;b&#39;);
title(&#39;The Unit Step Signal&#39;);


The unit ramp signal
A signal whose magnitude increases same as time.It can be obtained by integrating
unit step.

N=13;
a=0:1:N-1;
b=a;
subplot(3,2,3);
stem(a,b,&#39;b&#39;);
xlabel(&#39;a&#39;);
ylabel(&#39;b&#39;);
title(&#39;The Unit Ramp Signal&#39;);


The exponential signal:
The exponential signal is a sequence of the form
x(n) = a&quot; for all n
If the parameter a is real, then x( n )is a real signal. When the parameter a is
complex then x ( n )is a complex.

N=13;
a=0:1:N-1;
b=exp(a);
subplot(3,2,4);

stem(a,b,&#39;b&#39;);
xlabel(&#39;a&#39;);
ylabel(&#39;b&#39;);
title(&#39;The Exponential Signal&#39;);


Sinusoidal Signal:
A sine wave or sinusoid is a mathematical curve that describes a smooth periodic
oscillation. A sine wave is a continuous wave.

N=13;
a=0:1:N-1;
b=sin(.2*pi*a);
subplot(3,2,5);
stem(a,b,&#39;b&#39;);
xlabel(&#39;a&#39;);
ylabel(&#39;b&#39;);
title(&#39;Sinusoidal Signal&#39;);


Cosine Signal:
A cosine wave and its corresponding sine wave have the same frequency, but the
cosine wave leads the sine wave by 90 degrees of phase.

N=13;
a=0:1:N-1;
b=cos(.2*pi*a);
subplot(3,2,6);
stem(a,b,&#39;b&#39;);
xlabel(&#39;a&#39;);
ylabel(&#39;b&#39;);
title(&#39;Cosine Signal&#39;);
