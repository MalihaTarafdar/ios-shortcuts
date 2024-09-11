# BAC Calculator v1.0

## Installation
Install from iCloud link: [https://www.icloud.com/shortcuts/34ecbd152db04e3d80c5a0b148e6cf23](https://www.icloud.com/shortcuts/34ecbd152db04e3d80c5a0b148e6cf23)

**Note**: If you are on iOS 14 or lower, you must allow untrusted shortcuts in order to import this shortcut. To find out how, see [https://support.apple.com/guide/shortcuts/enable-shared-shortcuts-apdfeb05586f/4.0/ios/14.0](https://support.apple.com/guide/shortcuts/enable-shared-shortcuts-apdfeb05586f/4.0/ios/14.0). 

Install manually by saving `BAC Calculator.shortcut`. Then, import it by opening the file. 

## Usage
This shortcut uses the Widmark equation to estimate Blood Alcohol Content (BAC). It also approximates time until sobriety and includes information about the stages of alcohol intoxication and tips for safe drinking. For more information about Blood Alcohol Content, see [https://en.wikipedia.org/wiki/Blood_alcohol_content](https://en.wikipedia.org/wiki/Blood_alcohol_content). 

Information about the stages of alcohol intoxication is from the following study: [https://www.researchgate.net/publication/15751585_Alcohol_Determination_in_the_Clinical_Laboratory](https://www.researchgate.net/publication/15751585_Alcohol_Determination_in_the_Clinical_Laboratory)

## Widmark Equation
The Widmark equation is as follows. 
```math
N = \frac{Wr(C_t + \beta t)}{dz}
```
where
- $N$ is the number of standard drinks consumed
- $W$ is body weight
- $r$ is the constant for volume of distribution (of water in the body)
- $C_t$ is Blood Alcohol Content
- $\beta$ is the alcohol elimination rate
- $t$ is the time since the first drink
- $d$ is the density of ethanol at $20^\circ \text{C}$ (room temperature)
- $z$ is the alcohol content per drink

The implementation of the Widmark equation in this shortcut uses an alcohol elimination rate of 0.015 and also uses US fluid ounces. More information about the implementation can be found in the shortcut source. 

### Standard Drinks
A standard drink is defined as
- 1.5 fl oz of a 80-proof spirit (~40% ABV)
- 5 fl oz of a table wine (~12% ABV)
- 8-9 fl oz of malt liquor (~7% ABV)
- 12 fl oz of regular beer (~5% ABV)

For more information about standard drinks, see [https://en.wikipedia.org/wiki/Standard_drink](https://en.wikipedia.org/wiki/Standard_drink). 

## Support Me
This shortcut along with others I have made are open source and can be found at [https://github.com/MalihaTarafdar/ios-shortcuts](https://github.com/MalihaTarafdar/ios-shortcuts). If you found this shortcut useful, please consider supporting me at [coindrop.to/malihatarafdar](https://coindrop.to/malihatarafdar)!
