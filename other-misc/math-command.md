# Math Command

{% hint style="warning" %}
This page is only used as a general overview and guide of the features in the `/math` command. There may be functions, variables or expressions that will work but are not listed below.
{% endhint %}

## Numbers

* Binary
* Octal
* Hexadecimal
* Unary
* Unary Zero
* Base 1-36 Literals
* Base N

## Random Numbers

#### Functions

* Uniform Continuous Distribution
* Uniform Discrete Distribution
* Normal Distribution
* User Provided List

#### Variables

* Integer
* Integer N \(-10^k &lt;= N &lt;= 10^k for k = 1, 2, ...,9\)
* Natural
* Natural N \(N &lt;= 10^k for k = 1, 2, ...,9\)
* Uniform Continuous Distribution U\(0,1\)
* Normal Distribution N\(0,1\)

## Units

* Length
* Distance
* Information \(Kb, Mb, Gb, etc\)
* Volume

{% hint style="info" %}
You can find a list of supported units [here](math-command.md#supported-units).
{% endhint %}

## Operators

#### General

* SIGMA Summation
* PI Product

#### Bitwise

* Unary
* AND
* Exclusive OR
* Inclusive OR
* Signed Left/Right Shift

## Functions

* Unary
* Binary
* Conditional
* n-argument
* Primality test
* Primes Count
* Prime Factorization
* Standard Deviation
* Mean Estimation
* Variance Estimation
* Probability Distribution
* Cumulative Distribution
* Binary Relation "="
* Binary Relation "&lt;" & "&gt;"
* Boolean Operator "OR"
* Boolean Operator "AND"

## Derivatives

* General
* Left/Right
* Complex Function \(Including alternative syntaxs\)
* Integrals

## Supported Metric Prefixes

* \[Y\]                                   \(4.0\)  Septillion / Yotta = 10^24
* \[sept\]                                \(4.0\)  Septillion / Yotta = 10^24
* \[Z\]                                   \(4.0\)  Sextillion / Zetta = 10^21
* \[sext\]                                \(4.0\)  Sextillion / Zetta = 10^21
* \[E\]                                   \(4.0\)  Quintillion / Exa = 10^18
* \[quint\]                               \(4.0\)  Quintillion / Exa = 10^18
* \[P\]                                   \(4.0\)  Quadrillion / Peta = 10^15
* \[quad\]                                \(4.0\)  Quadrillion / Peta = 10^15
* \[T\]                                   \(4.0\)  Trillion / Tera = 10^12
* \[tril\]                                \(4.0\)  Trillion / Tera = 10^12
* \[G\]                                   \(4.0\)  Billion / Giga = 10^9
* \[bil\]                                 \(4.0\)  Billion / Giga = 10^9
* \[M\]                                   \(4.0\)  Million / Mega = 10^6
* \[mil\]                                 \(4.0\)  Million / Mega = 10^6
* \[k\]                                   \(4.0\)  Thousand / Kilo = 10^3
* \[th\]                                  \(4.0\)  Thousand / Kilo = 10^3
* \[hecto\]                               \(4.0\)  Hundred / Hecto = 10^2
* \[hund\]                                \(4.0\)  Hundred / Hecto = 10^2
* \[deca\]                                \(4.0\)  Ten / Deca = 10
* \[ten\]                                 \(4.0\)  Ten / Deca = 10
* \[deci\]                                \(4.0\)  Tenth / Deci = 0.1
* \[centi\]                               \(4.0\)  Hundredth / Centi = 0.01
* \[milli\]                               \(4.0\)  Thousandth / Milli = 0.001
* \[mic\]                                 \(4.0\)  Millionth / Micro = 10^-6
* \[n\]                                   \(4.0\)  Billionth / Nano = 10^-9
* \[p\]                                   \(4.0\)  Trillionth / Pico = 10^-12
* \[f\]                                   \(4.0\)  Quadrillionth / Femto = 10^-15
* \[a\]                                   \(4.0\)  Quintillionth / Atoo = 10^-18
* \[z\]                                   \(4.0\)  Sextillionth / Zepto = 10^-21
* \[y\]                                   \(4.0\)  Septillionth / Yocto = 10^-24

## Supported Constants

* pi                          Pi, Archimedes' constant or Ludolph's number
* e                           Napier's constant, or Euler's number, base of Natural logarithm
* \[gam\]                       Euler-Mascheroni constant
* \[phi\]                       Golden ratio
* \[PN\]                        Plastic constant
* \[B\*\]                        Embree-Trefethen constant
* \[F'd\]                       Feigenbaum constant alfa
* \[F'a\]                       Feigenbaum constant delta
* \[C2\]                        Twin prime constant
* \[M1\]                        Meissel-Mertens constant
* \[B2\]                        Brun's constant for twin primes
* \[B4\]                        Brun's constant for prime quadruplets
* \[BN'L\]                      de Bruijn-Newman constant
* \[Kat\]                       Catalan's constant
* \[K\*\]                        Landau-Ramanujan constant
* \[K.\]                        Viswanath's constant
* \[B'L\]                       Legendre's constant
* \[RS'm\]                      Ramanujan-Soldner constant
* \[EB'e\]                      Erdos-Borwein constant
* \[Bern\]                      Bernstein's constant
* \[GKW'l\]                     Gauss-Kuzmin-Wirsing constant
* \[HSM's\]                     Hafner-Sarnak-McCurley constant
* \[lm\]                        Golomb-Dickman constant
* \[Cah\]                       Cahen's constant
* \[Ll\]                        Laplace limit
* \[AG\]                        Alladi-Grinstead constant
* \[L\*\]                        Lengyel's constant
* \[L.\]                        Levy's constant
* \[Dz3\]                       Apery's constant
* \[A3n\]                       Mills' constant
* \[Bh\]                        Backhouse's constant
* \[Pt\]                        Porter's constant
* \[L2\]                        Lieb's square ice constant
* \[Nv\]                        Niven's constant
* \[Ks\]                        Sierpinski's constant
* \[Kh\]                        Khinchin's constant
* \[FR\]                        Fransen-Robinson constant
* \[La\]                        Landau's constant
* \[P2\]                        Parabolic constant
* \[Om\]                        Omega constant
* \[MRB\]                       MRB constant
* \[li2\]                       \(2.3\) li\(2\) - logarithmic integral function at x=2
* \[EG\]                        \(2.3\) Gompertz constant
* \[ c\]                        \(4.0\)  Light speed in vacuum \[m/s\] \(m=1, s=1\)
* \[G.\]                        \(4.0\)  Gravitational constant \(m=1, kg=1, s=1\)\]
* \[g\]                         \(4.0\)  Gravitational acceleration on Earth \[m/s^2\] \(m=1, s=1\)
* \[hP\]                        \(4.0\)  Planck constant \(m=1, kg=1, s=1\)
* \[h-\]                        \(4.0\)  Reduced Planck constant / Dirac constant \(m=1, kg=1, s=1\)\]
* \[lP\]                        \(4.0\)  Planck length \[m\] \(m=1\)
* \[mP\]                        \(4.0\)  Planck mass \[kg\] \(kg=1\)
* \[tP\]                        \(4.0\)  Planck time \[s\] \(s=1\)
* \[ly\]                        \(4.0\)  Light year \[m\] \(m=1\)
* \[au\]                        \(4.0\)  Astronomical unit \[m\] \(m=1\)
* \[pc\]                        \(4.0\)  Parsec \[m\] \(m=1\)
* \[kpc\]                       \(4.0\)  Kiloparsec \[m\] \(m=1\)
* \[Earth-R-eq\]                \(4.0\)  Earth equatorial radius \[m\] \(m=1\)
* \[Earth-R-po\]                \(4.0\)  Earth polar radius \[m\] \(m=1\)
* \[Earth-R\]                   \(4.0\)  Earth mean radius \(m=1\)
* \[Earth-M\]                   \(4.0\)  Earth mass \[kg\] \(kg=1\)
* \[Earth-D\]                   \(4.0\)  Earth-Sun distance - semi major axis \[m\] \(m=1\)
* \[Moon-R\]                    \(4.0\)  Moon mean radius \[m\] \(m=1\)
* \[Moon-M\]                    \(4.0\)  Moon mass \[kg\] \(kg=1\)
* \[Moon-D\]                    \(4.0\)  Moon-Earth distance - semi major axis \[m\] \(m=1\)
* \[Solar-R\]                   \(4.0\)  Solar mean radius \[m\] \(m=1\)
* \[Solar-M\]                   \(4.0\)  Solar mass \[kg\] \(kg=1\)
* \[Mercury-R\]                 \(4.0\)  Mercury mean radius \[m\] \(m=1\)
* \[Mercury-M\]                 \(4.0\)  Mercury mass \[kg\] \(kg=1\)
* \[Mercury-D\]                 \(4.0\)  Mercury-Sun distance - semi major axis \[m\] \(m=1\)
* \[Venus-R\]                   \(4.0\)  Venus mean radius \[m\] \(m=1\)
* \[Venus-M\]                   \(4.0\)  Venus mass \[kg\] \(kg=1\)
* \[Venus-D\]                   \(4.0\)  Venus-Sun distance - semi major axis \[m\] \(m=1\)
* \[Mars-R\]                    \(4.0\)  Mars mean radius \[m\] \(m=1\)
* \[Mars-M\]                    \(4.0\)  Mars mass \[kg\] \(kg=1\)
* \[Mars-D\]                    \(4.0\)  Mars-Sun distance - semi major axis \[m\] \(m=1\)
* \[Jupiter-R\]                 \(4.0\)  Jupiter mean radius \[m\] \(m=1\)
* \[Jupiter-M\]                 \(4.0\)  Jupiter mass \[kg\] \(kg=1\)
* \[Jupiter-D\]                 \(4.0\)  Jupiter-Sun distance - semi major axis \[m\] \(m=1\)
* \[Saturn-R\]                  \(4.0\)  Saturn mean radius \[m\] \(m=1\)
* \[Saturn-M\]                  \(4.0\)  Saturn mass \[kg\] \(kg=1\)
* \[Saturn-D\]                  \(4.0\)  Saturn-Sun distance - semi major axis \[m\] \(m=1\)
* \[Uranus-R\]                  \(4.0\)  Uranus mean radius \[m\] \(m=1\)
* \[Uranus-M\]                  \(4.0\)  Uranus mass \[kg\] \(kg=1\)
* \[Uranus-D\]                  \(4.0\)  Uranus-Sun distance - semi major axis \[m\] \(m=1\)
* \[Neptune-R\]                 \(4.0\)  Neptune mean radius \[m\] \(m=1\)
* \[Neptune-M\]                 \(4.0\)  Neptune mass \[kg\] \(kg=1\)
* \[Neptune-D\]                 \(4.0\)  Neptune-Sun distance - semi major axis \[m\] \(m=1\)

## Supported Units

* ulp                         \(3.0\) Unit in The Last Place - ulp\(0.1\)
* \[au\]                        \(4.0\)  Astronomical unit \[m\] \(m=1\)
* \[%\]                                   \(4.0\)  Percentage = 0.01
* \[%%\]                                  \(4.0\)  Promil, Per mille = 0.001
* \[Y\]                                   \(4.0\)  Septillion / Yotta = 10^24
* \[sept\]                                \(4.0\)  Septillion / Yotta = 10^24
* \[Z\]                                   \(4.0\)  Sextillion / Zetta = 10^21
* \[sext\]                                \(4.0\)  Sextillion / Zetta = 10^21
* \[E\]                                   \(4.0\)  Quintillion / Exa = 10^18
* \[quint\]                               \(4.0\)  Quintillion / Exa = 10^18
* \[P\]                                   \(4.0\)  Quadrillion / Peta = 10^15
* \[quad\]                                \(4.0\)  Quadrillion / Peta = 10^15
* \[T\]                                   \(4.0\)  Trillion / Tera = 10^12
* \[tril\]                                \(4.0\)  Trillion / Tera = 10^12
* \[G\]                                   \(4.0\)  Billion / Giga = 10^9
* \[bil\]                                 \(4.0\)  Billion / Giga = 10^9
* \[M\]                                   \(4.0\)  Million / Mega = 10^6
* \[mil\]                                 \(4.0\)  Million / Mega = 10^6
* \[k\]                                   \(4.0\)  Thousand / Kilo = 10^3
* \[th\]                                  \(4.0\)  Thousand / Kilo = 10^3
* \[hecto\]                               \(4.0\)  Hundred / Hecto = 10^2
* \[hund\]                                \(4.0\)  Hundred / Hecto = 10^2
* \[deca\]                                \(4.0\)  Ten / Deca = 10
* \[ten\]                                 \(4.0\)  Ten / Deca = 10
* \[deci\]                                \(4.0\)  Tenth / Deci = 0.1
* \[centi\]                               \(4.0\)  Hundredth / Centi = 0.01
* \[milli\]                               \(4.0\)  Thousandth / Milli = 0.001
* \[mic\]                                 \(4.0\)  Millionth / Micro = 10^-6
* \[n\]                                   \(4.0\)  Billionth / Nano = 10^-9
* \[p\]                                   \(4.0\)  Trillionth / Pico = 10^-12
* \[f\]                                   \(4.0\)  Quadrillionth / Femto = 10^-15
* \[a\]                                   \(4.0\)  Quintillionth / Atoo = 10^-18
* \[z\]                                   \(4.0\)  Sextillionth / Zepto = 10^-21
* \[y\]                                   \(4.0\)  Septillionth / Yocto = 10^-24
* \[m\]                                   \(4.0\)  Metre / Meter \(m=1\)
* \[km\]                                  \(4.0\)  Kilometre / Kilometer \(m=1\)
* \[cm\]                                  \(4.0\)  Centimetre / Centimeter \(m=1\)
* \[mm\]                                  \(4.0\)  Millimetre / Millimeter \(m=1\)
* \[inch\]                                \(4.0\)  Inch \(m=1\)
* \[yd\]                                  \(4.0\)  Yard \(m=1\)
* \[ft\]                                  \(4.0\)  Feet \(m=1\)
* \[mile\]                                \(4.0\)  Mile \(m=1\)
* \[nmi\]                                 \(4.0\)  Nautical mile \(m=1\)
* \[m2\]                                  \(4.0\)  Square metre / Square meter \(m=1\)
* \[cm2\]                                 \(4.0\)  Square centimetre / Square centimeter \(m=1\)
* \[mm2\]                                 \(4.0\)  Square millimetre / Square millimeter \(m=1\)
* \[are\]                                 \(4.0\)  Are \(m=1\)
* \[ha\]                                  \(4.0\)  Hectare \(m=1\)
* \[acre\]                                \(4.0\)  Acre \(m=1\)
* \[km2\]                                 \(4.0\)  Square kilometre / Square kilometer \(m=1\)
* \[mm3\]                                 \(4.0\)  Cubic millimetre / Cubic millimeter \(m=1\)
* \[cm3\]                                 \(4.0\)  Cubic centimetre / Cubic centimeter \(m=1\)
* \[m3\]                                  \(4.0\)  Cubic metre / Cubic meter \(m=1\)
* \[km3\]                                 \(4.0\)  Cubic kilometre / Cubic kilometer \(m=1\)
* \[ml\]                                  \(4.0\)  Millilitre / Milliliter \(m=1\)
* \[l\]                                   \(4.0\)  Litre / Liter \(m=1\)
* \[gall\]                                \(4.0\)  Gallon \(m=1\)
* \[pint\]                                \(4.0\)  Pint \(m=1\)
* \[s\]                                   \(4.0\)  Second \(s=1\)
* \[ms\]                                  \(4.0\)  Millisecond \(s=1\)
* \[min\]                                 \(4.0\)  Minute \(s=1\)
* \[h\]                                   \(4.0\)  Hour \(s=1\)
* \[day\]                                 \(4.0\)  Day \(s=1\)
* \[week\]                                \(4.0\)  Week \(s=1\)
* \[yearj\]                               \(4.0\)  Julian year = 365.25 days \(s=1\)
* \[kg\]                                  \(4.0\)  Kilogram \(kg=1\)
* \[gr\]                                  \(4.0\)  Gram \(kg=1\)
* \[mg\]                                  \(4.0\)  Milligram \(kg=1\)
* \[dag\]                                 \(4.0\)  Decagram \(kg=1\)
* \[t\]                                   \(4.0\)  Tonne \(kg=1\)
* \[oz\]                                  \(4.0\)  Ounce \(kg=1\)
* \[lb\]                                  \(4.0\)  Pound \(kg=1\)
* \[b\]                                   \(4.0\)  Bit \(bit=1\)
* \[kb\]                                  \(4.0\)  Kilobit \(bit=1\)
* \[Mb\]                                  \(4.0\)  Megabit \(bit=1\)
* \[Gb\]                                  \(4.0\)  Gigabit \(bit=1\)
* \[Tb\]                                  \(4.0\)  Terabit \(bit=1\)
* \[Pb\]                                  \(4.0\)  Petabit \(bit=1\)
* \[Eb\]                                  \(4.0\)  Exabit \(bit=1\)
* \[Zb\]                                  \(4.0\)  Zettabit \(bit=1\)
* \[Yb\]                                  \(4.0\)  Yottabit \(bit=1\)
* \[B\]                                   \(4.0\)  Byte \(bit=1\)
* \[kB\]                                  \(4.0\)  Kilobyte \(bit=1\)
* \[MB\]                                  \(4.0\)  Megabyte \(bit=1\)
* \[GB\]                                  \(4.0\)  Gigabyte \(bit=1\)
* \[TB\]                                  \(4.0\)  Terabyte \(bit=1\)
* \[PB\]                                  \(4.0\)  Petabyte \(bit=1\)
* \[EB\]                                  \(4.0\)  Exabyte \(bit=1\)
* \[ZB\]                                  \(4.0\)  Zettabyte \(bit=1\)
* \[YB\]                                  \(4.0\)  Yottabyte \(bit=1\)
* \[J\]                                   \(4.0\)  Joule \(m=1, kg=1, s=1\)
* \[eV\]                                  \(4.0\)  Electronovolt \(m=1, kg=1, s=1\)
* \[keV\]                                 \(4.0\)  Kiloelectronovolt \(m=1, kg=1, s=1\)
* \[MeV\]                                 \(4.0\)  Megaelectronovolt \(m=1, kg=1, s=1\)
* \[GeV\]                                 \(4.0\)  Gigaelectronovolt \(m=1, kg=1, s=1\)
* \[TeV\]                                 \(4.0\)  Teraelectronovolt \(m=1, kg=1, s=1\)
* \[m/s\]                                 \(4.0\)  Metre / Meter per second \(m=1, s=1\)
* \[km/h\]                                \(4.0\)  Kilometre / Kilometer per hour \(m=1, s=1\)
* \[mi/h\]                                \(4.0\)  Mile per hour \(m=1, s=1\)
* \[knot\]                                \(4.0\)  Knot \(m=1, s=1\)
* \[m/s2\]                                \(4.0\)  Metre / Meter per square second \(m=1, s=1\)
* \[km/h2\]                               \(4.0\)  Kilometre / Kilometer per square hour \(m=1, s=1\)
* \[mi/h2\]                               \(4.0\)  Mile per square hour \(m=1, s=1\)
* \[rad\]                                 \(4.0\)  Radian \(rad=1\)
* \[deg\]                                 \(4.0\)  Degree of arc \(rad=1\)
* \['\]                                   \(4.0\)  Minute of arc \(rad=1\)
* \[''\]                                  \(4.0\)  Second of arc \(rad=1\)

