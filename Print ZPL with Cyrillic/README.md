# Printing Cyrillic using ZPL code
While printing labels on a TSC ML340P printer, we encountered a problem with slow printing of Cyrillic letters using ZPL code.

## Test case "Comparative printing of Cyrillic and Latin characters using ZPL code":
- 01 Fonts TTF.zip              -- fonts to load into the ML340P TSC printer
- 02 TSC file fonts.png         -- ML340P TSC printer settings
- 03 TSC Native print slow.png  -- native print ZPL code with Cyrillic in Diagnostic Tool 1.63
- 04 ZPL Native slow.zpl        -- native ZPL code with Cyrillic characters to print
- 05 ZPL Cyrillic convert.zpl   -- Cyrillic converted ZPL code
- 06 ZPL Latin convert.zpl      -- converted Latin ZPL code
- 07 ZPL Native fast.zpl        -- native ZPL code with Latin characters for printing
- 08 TSC Native fast.png        -- native print ZPL code with Latin characters in Diagnostic Tool 1.63
- 09 TSC print labels.jpg       -- printed labels on the TSC ML340P printer

![](02%20TSC%20file%20fonts.png?raw=true)
![](03%20TSC%20Native%20print%20slow.png?raw=true)
![](04%20ZPL%20Native%20slow.zpl?raw=true)
![](05%20ZPL%20Cyrillic%20convert.zpl?raw=true)
![](06%20ZPL%20Latin%20convert.zpl?raw=true)
![](07%20ZPL%20Native%20fast.zpl?raw=true)
![](08%20TSC%20Native%20fast.png?raw=true)
![](09%20TSC%20print%20labels.jpg?raw=true)
