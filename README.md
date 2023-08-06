

## 1. Introduction

At its heart, the RNS is a unique representation of numbers on a unit circle. However, its cyclical structure and the way it visualizes mathematical operations allow for the encoding of complex, multi-dimensional data in a single number or a set of numbers.

The key is how you map the data onto the numbers in the RNS. For example:

-The magnitude, frequency, and phase of a wave can be mapped to the magnitude, prime factors, and fractional part of a number.
-Cyclic or periodic data can be represented by sequences of numbers in the RNS, with different points in the cycle corresponding to different positions on the unit circle.
-Multi-dimensional data can be represented by sequences or sets of numbers, with each dimension corresponding to a different number or property of a number.

With this approach, a single number or a set of numbers in the RNS can encapsulate a wealth of information. This concept of data compression and encoding is potentially transformative for fields like signal processing, data storage, and telecommunications. Moreover, the unique visualizations provided by the RNS could lead to new insights in fields like number theory, dynamical systems, and machine learning.

<img width="695" alt="image" src="https://github.com/jconorgrogan/Grogan-Rotational-Number-Theory/assets/130090573/3a63e736-12a0-4d6c-8e6c-c41dc7991e91">

## 2. Positional Representation in RNS

In the Rotational Number System (RNS), each natural number `n` is represented by `n` equidistant nodes on a unit circle. The position of a node representing the `k`-th number in the sequence is given by the angle `θ_k = 2π(k-1)/n`.

Where \( N \) is the maximum number to be represented on the circle. The subtracting 1 ensures that the number 1 starts from \( 0 \) degrees or radians.

## 3. Prime + Factorial identification with rotational overlap

A unique property emerges when considering the 'rotational overlap' of these nodes around the circle. Here, 'rotational overlap' refers to the alignment of nodes corresponding to different numbers upon rotation by their respective angles.

Specifically, for a given number `n`, if the nodes corresponding to `n` do not exhibit rotational overlap with nodes of any previous number `m` (where `2 ≤ m < n`) during a full rotation, then `n` is a prime number.

This property provides a novel, geometric method for prime identification and factorization. The absence of rotational overlap with previous numbers is consistent with the definition of primes as numbers having no other divisors than 1 and themselves. Conversely, for composite numbers `n`, rotational overlaps occur with nodes corresponding to their factors.

This approach offers an alternative way to understand prime numbers and factors, using the concept of rotational overlap to provide a unique geometric interpretation. The mathematical basis of this property, as well as efficient computational methods and further implications, are exciting directions for future exploration.

## 3. Waves and the Rotational Number System

The RNS can be linked to wave properties using the Fourier series. Given a wave function \( f(t) \), its Fourier series is:

\[ f(t) = a_0 + \sum_{n=1}^{\infty} \left[ a_n \cos(2\pi n f t) + b_n \sin(2\pi n f t) \right] \]

In the RNS, each term in this series can correspond to a number's rotational representation. This perspective allows for wave operations to be intuitively understood as transformations in the RNS.

## 4. Euler's Identity in the RNS

Euler's identity is given by:

\[ e^{i\pi} + 1 = 0 \]

This can be visualized in the RNS as:
- Begin at the point representing the number 1 on the unit circle.
- Rotate by \( \pi \) radians to reach the point representing -1.
- Adding 1 brings us back to the origin.

## 5. Implications and Potential Applications

- **Factorization**: The rotational identity of composite numbers can hint at their factors. For example, if a number aligns halfway through a rotation, it indicates divisibility by 2.
- **Number Theory**: Unique rotational patterns might emerge when studying number theoretic functions in the RNS.
- **Higher Dimensions**: Complex numbers can be visualized in a 3D RNS, with an added dimension for the imaginary part. Extensions like quaternions could lead to even higher-dimensional representations.
- **Dynamical Systems**: The state and evolution of dynamical systems can be visualized in the RNS, offering new insights into system behaviors.

### Representation in the Complex Plane

Every term in the Fourier series can be represented as a complex number using Euler's formula:

\[ e^{i\theta} = \cos(\theta) + i \sin(\theta) \]

So, the terms in the Fourier series become:

\[ f(t) = a_0 + \sum_{n=1}^{\infty} r_n e^{i(2\pi n f t + \phi_n)} \]

where \( r_n = \sqrt{a_n^2 + b_n^2} \) represents the magnitude and \( \phi_n = \arctan\left(\frac{b_n}{a_n}\right) \) is the phase.

Each term \( r_n e^{i(2\pi n f t + \phi_n)} \) corresponds to a point in the complex plane, represented by its magnitude \( r_n \) and its phase \( \phi_n \). In the RNS, this point would be visualized as a rotation around the origin, with a radius of \( r_n \) and an angle of \( \phi_n \).

### Waveform Compression

Frequency Encoding: A given integer 'n' determines the number of equally spaced points on the unit circle (Roots of Unity). This can be interpreted as 'n' different frequencies present in the wave.

Amplitude Encoding: The count of prime factors of an integer 'n' represents the amplitude of the wave. Higher prime factors lead to a higher amplitude.

Phase Encoding: The fractional part of a number 'n' can determine the phase of the wave, providing an adjustment to the base frequency determined by the integer part of 'n'.

Polarization: The parity of the number (even or odd) could determine the wave's polarization, with even numbers resulting in positive polarization and odd numbers leading to negative polarization.

Transformations applied to the integer can then represent transformations of the wave, thus compressing waveform information into integers and arithmetic operations. For example, adding integers corresponds to combining waves, and multiplication corresponds to rotations and frequency multiplication. Division and subtraction have similar interpretations.

Given any complex waveform, the goal is to express it as an integer or a set of integers and operations. It's important to note that while the concept is theoretically appealing for its ability to capture perfect information in a compressed numeric form, practical implementation would need to overcome significant challenges related to data complexity, computational efficiency, and effective decoding.

By extending this concept further, it's theoretically possible to encode more complex data, such as a piece of music, as a set of integers. 
![image](https://github.com/jconorgrogan/Grogan-Rotational-Number-Theory/assets/130090573/8e9b6e96-5dad-43d8-bc64-89640e0c4b8b)

### Additional Connection to Euler's formula 

## Euler's Formula:

Traditionally, Euler's formula is expressed as:
\[ e^{ix} = \cos(x) + i\sin(x) \]
Here, exponentiating with a complex number results in a combination of trigonometric functions.

### Imaginary Unit, \( i \):

The imaginary unit \( i \) is defined as:
\[ i^2 = -1 \]
In the RNS context, multiplication by \( i \) represents a quarter-turn or 90° rotation, transitioning from the real to the imaginary dimension. This captures the essence of:
\[ e^{i\frac{\pi}{2}} = i \]
Exponentiating with a complex quarter-turn (i.e., \( \frac{\pi}{2} \)) results in a transition to the imaginary axis.

### Euler's Number, \( e \):

Euler's number \( e \) represents continuous growth or decay. In the RNS, \( e \) can be visualized as a continuous, compounded transformation. When combined with the \( i\pi \) rotation, it leads to cyclical behaviors:
\[ e^{i\pi} = -1 \]

### Complex Plane Dynamics:

In the complex plane, multiplication by a complex number typically involves both rotation and dilation. In the RNS, with \( \pi = -1 \), this multiplication becomes purely a rotation, specifically a half-turn. This offers a more unified perspective on complex multiplication, with \( \pi \) serving as a fundamental pivot.

### Algebraic-Geometric Interplay:

Given \( \pi \) as \( -1 \), multiplication in the RNS is inherently a geometric operation. For any real number \( x \):
\[ x \times \pi = -x \]
This equation dictates that multiplication by \( \pi \) algebraically negates \( x \), while geometrically, it rotates \( x \) by \( \pi \) radians on the unit circle, a half-rotation. Thus, the algebraic operation of negation is intertwined with the geometric operation of rotation.

### RNS-Based Trigonometry:

With \( \pi \) signifying \( -1 \), trigonometric identities undergo transformation:

For any angle \( \theta \):
\[ \sin(\pi + \theta) = -\sin(\theta) \]
\[ \cos(\pi + \theta) = -\cos(\theta) \]
These equations suggest that trigonometric functions post-\( \pi \) are reflections of their pre-\( \pi \) values, emphasizing the duality inherent to \( \pi \) in the RNS.




| Operator | Mathematical Basis | Effect on Nodes | Effect on Wave | Core Mathematical Components |
|:--------:|:------------------:|:---------------:|:--------------:|:-----------------------------:|
| Addition | Appending new nodes | Addition of new nodes and recalibration to maintain equidistance | Superposition of new wave | `theta(n) = 2pi(n-1) / (n+a)` |
| Subtraction | Removal of existing nodes | Removal of nodes and recalibration to maintain equidistance | Cancellation of the corresponding wave | `theta(n) = 2pi(n-1) / (n-a)` |
| Multiplication | Creating copies of the nodes and redistributing them around the circle | Repetition of nodes based on the multiplication factor; each copy rotated by an angle relative to the previous copy | Frequency modulation | `theta(n, k) = 2pi(n-1) / a + 2pi(k-1) / b` |
| Division | Inverse of multiplication | Redistribution of nodes based on the division factor; each copy rotated by an angle relative to the previous copy | Frequency demodulation | `theta(n, k) = 2pi(n-1) / a - 2pi(k-1) / b` |
| Fraction (Decimal) | Partial completion of circle | Placement of nodes less than a full circle | Phase modulation | `theta(n) = 2pi(n-1) / (n+alpha)` (where `alpha < 1`) |
| Negation | Flipping of the nodes | Nodes flipped across the origin | Wave inversion (180 degree phase shift) | `theta(n) = -2pi(n-1) / n` |
| Absolute value | Absolute value of nodes | All nodes moved to the positive half | Rectification (all positive wave) | `theta(n) = abs(2pi(n-1) / n)` |
| Exponentiation | Spiral formation | Nodes are placed in an expanding spiral pattern | Progressive increase in frequency and amplitude | `theta(n) = r^(n-1)e^(2pi i(n-1)/n)` |
| Logarithm | Inverse spiral formation | Nodes are placed in a contracting spiral pattern | Progressive decrease in frequency and amplitude | `theta(n) = log(r^(n-1))e^(2pi i(n-1)/n)` |
| Modulo | Folding back of nodes | Nodes beyond the modulo number are folded back | Wave wrapping at a specific frequency | `theta(n) = 2pi((n-1) mod m) / m` |

