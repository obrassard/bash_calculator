# bash_calculator
[![Hex.pm](https://img.shields.io/badge/Compatible With-Mac OS & Linux-brightgreen.svg)]()
[![Hex.pm](https://img.shields.io/badge/Version-1.1.0-blue.svg)]()

_Calculate basic operations right from your bash terminal !_ - [Created by Olivier Brassard]
(https://github.com/obrassard)
___
### Instructions

Simply copy the shell script **calcul** to one of the *bin* repository recorded in your $PATH. [!Be sure you can execute the file.](https://github.com/obrassard/bash_calculator/wiki/Troubleshooting)
```shell
# Remember that you can use this command to see what repository are recorder in $PATH
echo $PATH
```
**!** On v1.1.0 and above we partially based the script on *bc* command processor to be able to calculate decimals. Thus, for everything to work, *bc* must be installed on your system. [See this page if bc isn't installed on your system.](https://github.com/obrassard/bash_calculator/wiki/Troubleshooting)

Open a new terminal for changes to be applied.
___
### Usage
Once installed use **calcul** command to perform simple calculation ( +, - , x, or / )

When you write the command you must include [+, -, x, or /] as the first parameter, followed by the numbers you want (separated by space).
Use **-n** argument to get the answer without text:
```shell
hostname:~ user$ calcul -n + 1 2 3
6
```
#### Addition
Use the [ + ] parameter.
```shell
calcul + 23 42 53
```
#### Substraction
Use the [ - ] parameter.
The script substract numbers from left to right:
```shell
calcul - 5 3 2
```
This would calculate ( 5 - 3 - 2 ).
#### Multiplication
Use the [ x ] parameter.
```shell
calcul x 2 4 6
```
#### Division
Use the [ / ] parameter.
The script divide numbers from left to right:
```shell
calcul / 10.5 2
```
This would calculate ( 10.5 / 2 ).

#### Modulo
Use the [ % ] parameter.
Modulo only works with two numbers; w/o decimal.
```shell
calcul % 11 2
```
This would calculate ( 11 MOD 2 ).

#### Exponent
Use the [ ex ] parameter.
Exponent only works with two numbers; w/o decimal
```shell
calcul ex 3 2
```
This would calculate ( 3^2 ).

### Squareroot
Use the [ sqr ] parameter.
Square root works with one number, and you can use decimal.
```shell
calcul sqr 9
```
___
### Troubleshooting

If you can't use the command please [visit this page](https://github.com/obrassard/bash_calculator/wiki/Troubleshooting)
___
You can use this command at any time to find these instructions
```shell
calcul help
```
