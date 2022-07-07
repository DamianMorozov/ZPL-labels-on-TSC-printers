# Printing Cyrillic using ZPL code
While printing labels on a TSC ML340P printer, we encountered a problem with slow printing of Cyrillic letters using ZPL code.

- [Back to the Home](../README.md)

## Test case "Comparative printing of Cyrillic and Latin characters using ZPL code":
- 01 Fonts TTF.zip              -- fonts to load into the ML340P TSC printer
- 02 TSC file fonts.png         -- ML340P TSC printer settings
- 03 TSC Native print slow.png  -- native print ZPL code with Cyrillic in Diagnostic Tool 1.63
- 04 ZPL Native slow.zpl        -- native ZPL code with Cyrillic characters to print
- 05 ZPL Cyrillic convert.zpl   -- Cyrillic converted ZPL code
- 06 ZPL Latin convert.zpl      -- converted Latin ZPL code
- 07 ZPL Native fast.zpl        -- native ZPL code with Latin characters for printing
- 08 TSC Native fast.png        -- native print ZPL code with Latin characters in Diagnostic Tool 1.63
- 09 TSC print labels.png       -- printed labels on the TSC ML340P printer

![](02%20TSC%20file%20fonts.png?raw=true)
![](03%20TSC%20Native%20print%20slow.png?raw=true)
![](04%20ZPL%20Native%20slow.zpl?raw=true)
![](05%20ZPL%20Cyrillic%20convert.zpl?raw=true)
![](06%20ZPL%20Latin%20convert.zpl?raw=true)
![](07%20ZPL%20Native%20fast.zpl?raw=true)
![](08%20TSC%20Native%20fast.png?raw=true)
![](09%20TSC%20print%20labels.png?raw=true)

## ZPL convert from Native into Cyrillic
1. Copy and paste ZPL into Notepad++.
2. Select data (Example: "31_37_2E_30_36_2E_32_30_32_32_0D_0A").
3. Ctrl + H:
	Find what: "_"
	Replace with: ""
	Search mode: Normal
	✓ In selection.
4. Plugins → Converter → HEX → ASCII.

- [Text Cyrillic to Latin](https://www.branah.com/cyrillic-to-latin)

## ZPL convert from Latin into Native
1. Copy and paste ZPL into Notepad++.
2. Select data (Example: "Data izgot.:").
3. Plugins → Converter → ASCII → HEX.
4. Select data (Example: "4461746120697A676F742E3A").
5. Ctrl + H:
	Find what: (..)
	Replace with: _\1
	Search mode: Regular expression
	✓ In selection.
6. Plugins → Converter → HEX → ASCII.
