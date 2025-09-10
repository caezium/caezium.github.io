


## Circuit Components & Special Resistors

- **LDR (Light-Dependent Resistor):** Resistance decreases when light increases
- **Thermistors (NTC):** Resistance decreases as temperature increases
- Both used as sensors in circuits



![[02_areas/PHYSICS/4/attachments/727fa2ced6e6242521e7784de9e8128d_MD5.jpg]]

---

### Potential Divider

- Two resistors in series divide voltage:

$V_1 = V_{in} \times \frac{R_1}{R_1 + R_2}$
$V_2 = V_{in} \times \frac{R_2}{R_1 + R_2}$

- Used to provide a fraction of voltage to another component
![[02_areas/PHYSICS/4/attachments/73e928a72d8f74e2e56df3c2d28e33de_MD5.jpg]]

- The potential difference across each resistor depends upon its resistance:
    
    - The resistor with the **largest resistance** will have a **greater potential difference** than the other one
        
    - If the **resistance** of one of the resistors is **increased**, it will get a **greater** share of the potential difference, whilst the **other** resistor will get a **smaller** share
        
- If one resistor is a **variable resistor**, the potential difference across the other resistor can be **altered**
    
    - This means the potential difference across any component **in parallel** with that resistor can also be altered
- - When two resistors are connected in series, the power source's e.m.f. is split between the resistors
    
    - This potential difference splits in the **same ratio** as the resistance of the two resistors
        
- The ratio of potential differences across each resistor can be found using the following equation:
    

![R subscript 1 over R subscript 2 space equals space V subscript 1 over V subscript 2](data:image/svg+xml;charset=utf8,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20xmlns%3Awrs%3D%22http%3A%2F%2Fwww.wiris.com%2Fxml%2Fmathml-extension%22%20height%3D%2259%22%20width%3D%2283%22%20wrs%3Abaseline%3D%2236%22%3E%3C!--MathML%3A%20%3Cmath%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F1998%2FMath%2FMathML%22%3E%3Cmfrac%3E%3Cmsub%3E%3Cmi%3ER%3C%2Fmi%3E%3Cmn%3E1%3C%2Fmn%3E%3C%2Fmsub%3E%3Cmsub%3E%3Cmi%3ER%3C%2Fmi%3E%3Cmn%3E2%3C%2Fmn%3E%3C%2Fmsub%3E%3C%2Fmfrac%3E%3Cmo%3E%26%23xA0%3B%3C%2Fmo%3E%3Cmo%3E%3D%3C%2Fmo%3E%3Cmo%3E%26%23xA0%3B%3C%2Fmo%3E%3Cmfrac%3E%3Cmsub%3E%3Cmi%3EV%3C%2Fmi%3E%3Cmn%3E1%3C%2Fmn%3E%3C%2Fmsub%3E%3Cmsub%3E%3Cmi%3EV%3C%2Fmi%3E%3Cmn%3E2%3C%2Fmn%3E%3C%2Fmsub%3E%3C%2Fmfrac%3E%3C%2Fmath%3E--%3E%3Cdefs%3E%3Cstyle%20type%3D%22text%2Fcss%22%3E%40font-face%7Bfont-family%3A'math17f39f8317fbdb1988ef4c628eb'%3Bsrc%3Aurl\(data%3Afont%2Ftruetype%3Bcharset%3Dutf-8%3Bbase64%2CAAEAAAAMAIAAAwBAT1MvMi7iBBMAAADMAAAATmNtYXDEvmKUAAABHAAAADRjdnQgDVUNBwAAAVAAAAA6Z2x5ZoPi2VsAAAGMAAAAsmhlYWQQC2qxAAACQAAAADZoaGVhCGsXSAAAAngAAAAkaG10eE2rRkcAAAKcAAAACGxvY2EAHTwYAAACpAAAAAxtYXhwBT0FPgAAArAAAAAgbmFtZaBxlY4AAALQAAABn3Bvc3QB9wD6AAAEcAAAACBwcmVwa1uragAABJAAAAAUAAADSwGQAAUAAAQABAAAAAAABAAEAAAAAAAAAQEAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACAgICAAAAAg1UADev96AAAD6ACWAAAAAAACAAEAAQAAABQAAwABAAAAFAAEACAAAAAEAAQAAQAAAD3%2F%2FwAAAD3%2F%2F%2F%2FEAAEAAAAAAAABVAMsAIABAABWACoCWAIeAQ4BLAIsAFoBgAKAAKAA1ACAAAAAAAAAACsAVQCAAKsA1QEAASsABwAAAAIAVQAAAwADqwADAAcAADMRIRElIREhVQKr%2FasCAP4AA6v8VVUDAAACAIAA6wLVAhUAAwAHAGUYAbAIELAG1LAGELAF1LAIELAB1LABELAA1LAGELAHPLAFELAEPLABELACPLAAELADPACwCBCwBtSwBhCwB9SwBxCwAdSwARCwAtSwBhCwBTywBxCwBDywARCwADywAhCwAzwxMBMhNSEdASE1gAJV%2FasCVQHAVdVVVQAAAAEAAAABAADVeM5BXw889QADBAD%2F%2F%2F%2F%2F1joTc%2F%2F%2F%2F%2F%2FWOhNzAAD%2FIASAA6sAAAAKAAIAAQAAAAAAAQAAA%2Bj%2FagAAF3AAAP%2B2BIAAAQAAAAAAAAAAAAAAAAAAAAIDUgBVA1YAgAAAAAAAAAAoAAAAsgABAAAAAgBeAAUAAAAAAAIAgAQAAAAAAAQAAN4AAAAAAAAAFQECAAAAAAAAAAEAEgAAAAAAAAAAAAIADgASAAAAAAAAAAMAMAAgAAAAAAAAAAQAEgBQAAAAAAAAAAUAFgBiAAAAAAAAAAYACQB4AAAAAAAAAAgAHACBAAEAAAAAAAEAEgAAAAEAAAAAAAIADgASAAEAAAAAAAMAMAAgAAEAAAAAAAQAEgBQAAEAAAAAAAUAFgBiAAEAAAAAAAYACQB4AAEAAAAAAAgAHACBAAMAAQQJAAEAEgAAAAMAAQQJAAIADgASAAMAAQQJAAMAMAAgAAMAAQQJAAQAEgBQAAMAAQQJAAUAFgBiAAMAAQQJAAYACQB4AAMAAQQJAAgAHACBAE0AYQB0AGgAIABGAG8AbgB0AFIAZQBnAHUAbABhAHIATQBhAHQAaABzACAARgBvAHIAIABNAG8AcgBlACAATQBhAHQAaAAgAEYAbwBuAHQATQBhAHQAaAAgAEYAbwBuAHQAVgBlAHIAcwBpAG8AbgAgADEALgAwTWF0aF9Gb250AE0AYQB0AGgAcwAgAEYAbwByACAATQBvAHIAZQAAAwAAAAAAAAH0APoAAAAAAAAAAAAAAAAAAAAAAAAAALkHEQAAjYUYALIAAAAVFBOxAAE%2F\)format\('truetype'\)%3Bfont-weight%3Anormal%3Bfont-style%3Anormal%3B%7Dtext%7Bfill%3A%23000000%3B%3C%2Fstyle%3E%3C%2Fdefs%3E%3Cline%20stroke%3D%22%23000000%22%20stroke-linecap%3D%22square%22%20stroke-width%3D%221%22%20x1%3D%222.5%22%20x2%3D%2225.5%22%20y1%3D%2229.5%22%20y2%3D%2229.5%22%2F%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2218%22%20font-style%3D%22italic%22%20text-anchor%3D%22middle%22%20x%3D%2210.5%22%20y%3D%2216%22%3ER%3C%2Ftext%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2213%22%20text-anchor%3D%22middle%22%20x%3D%2220.5%22%20y%3D%2224%22%3E1%3C%2Ftext%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2218%22%20font-style%3D%22italic%22%20text-anchor%3D%22middle%22%20x%3D%2210.5%22%20y%3D%2247%22%3ER%3C%2Ftext%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2213%22%20text-anchor%3D%22middle%22%20x%3D%2220.5%22%20y%3D%2255%22%3E2%3C%2Ftext%3E%3Ctext%20font-family%3D%22math17f39f8317fbdb1988ef4c628eb%22%20font-size%3D%2216%22%20text-anchor%3D%22middle%22%20x%3D%2240.5%22%20y%3D%2236%22%3E%3D%3C%2Ftext%3E%3Cline%20stroke%3D%22%23000000%22%20stroke-linecap%3D%22square%22%20stroke-width%3D%221%22%20x1%3D%2255.5%22%20x2%3D%2279.5%22%20y1%3D%2229.5%22%20y2%3D%2229.5%22%2F%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2218%22%20font-style%3D%22italic%22%20text-anchor%3D%22middle%22%20x%3D%2263.5%22%20y%3D%2216%22%3EV%3C%2Ftext%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2213%22%20text-anchor%3D%22middle%22%20x%3D%2274.5%22%20y%3D%2224%22%3E1%3C%2Ftext%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2218%22%20font-style%3D%22italic%22%20text-anchor%3D%22middle%22%20x%3D%2263.5%22%20y%3D%2247%22%3EV%3C%2Ftext%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2213%22%20text-anchor%3D%22middle%22%20x%3D%2274.5%22%20y%3D%2255%22%3E2%3C%2Ftext%3E%3C%2Fsvg%3E)

- Where:
    
    - ![R subscript 1](data:image/svg+xml;charset=utf8,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20xmlns%3Awrs%3D%22http%3A%2F%2Fwww.wiris.com%2Fxml%2Fmathml-extension%22%20height%3D%2228%22%20width%3D%2221%22%20wrs%3Abaseline%3D%2216%22%3E%3C!--MathML%3A%20%3Cmath%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F1998%2FMath%2FMathML%22%3E%3Cmsub%3E%3Cmi%3ER%3C%2Fmi%3E%3Cmn%3E1%3C%2Fmn%3E%3C%2Fmsub%3E%3C%2Fmath%3E--%3E%3Cdefs%3E%3Cstyle%20type%3D%22text%2Fcss%22%3Etext%7Bfill%3A%23000000%3B%7D%3C%2Fstyle%3E%3C%2Fdefs%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2218%22%20font-style%3D%22italic%22%20text-anchor%3D%22middle%22%20x%3D%226.5%22%20y%3D%2216%22%3ER%3C%2Ftext%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2213%22%20text-anchor%3D%22middle%22%20x%3D%2216.5%22%20y%3D%2224%22%3E1%3C%2Ftext%3E%3C%2Fsvg%3E) is the resistance of resistor 1 in ohms, Ω
        
    - ![R subscript 2](data:image/svg+xml;charset=utf8,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20xmlns%3Awrs%3D%22http%3A%2F%2Fwww.wiris.com%2Fxml%2Fmathml-extension%22%20height%3D%2228%22%20width%3D%2221%22%20wrs%3Abaseline%3D%2216%22%3E%3C!--MathML%3A%20%3Cmath%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F1998%2FMath%2FMathML%22%3E%3Cmsub%3E%3Cmi%3ER%3C%2Fmi%3E%3Cmn%3E2%3C%2Fmn%3E%3C%2Fmsub%3E%3C%2Fmath%3E--%3E%3Cdefs%3E%3Cstyle%20type%3D%22text%2Fcss%22%3Etext%7Bfill%3A%23000000%3B%7D%3C%2Fstyle%3E%3C%2Fdefs%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2218%22%20font-style%3D%22italic%22%20text-anchor%3D%22middle%22%20x%3D%226.5%22%20y%3D%2216%22%3ER%3C%2Ftext%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2213%22%20text-anchor%3D%22middle%22%20x%3D%2216.5%22%20y%3D%2224%22%3E2%3C%2Ftext%3E%3C%2Fsvg%3E) is the resistance of resistor 2 in ohms, Ω
        
    - ![V subscript 1](data:image/svg+xml;charset=utf8,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20xmlns%3Awrs%3D%22http%3A%2F%2Fwww.wiris.com%2Fxml%2Fmathml-extension%22%20height%3D%2228%22%20width%3D%2222%22%20wrs%3Abaseline%3D%2216%22%3E%3C!--MathML%3A%20%3Cmath%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F1998%2FMath%2FMathML%22%3E%3Cmsub%3E%3Cmi%3EV%3C%2Fmi%3E%3Cmn%3E1%3C%2Fmn%3E%3C%2Fmsub%3E%3C%2Fmath%3E--%3E%3Cdefs%3E%3Cstyle%20type%3D%22text%2Fcss%22%3Etext%7Bfill%3A%23000000%3B%7D%3C%2Fstyle%3E%3C%2Fdefs%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2218%22%20font-style%3D%22italic%22%20text-anchor%3D%22middle%22%20x%3D%226.5%22%20y%3D%2216%22%3EV%3C%2Ftext%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2213%22%20text-anchor%3D%22middle%22%20x%3D%2217.5%22%20y%3D%2224%22%3E1%3C%2Ftext%3E%3C%2Fsvg%3E) is the potential difference across resistor 1 in volts, V
        
    - ![V subscript 2](data:image/svg+xml;charset=utf8,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20xmlns%3Awrs%3D%22http%3A%2F%2Fwww.wiris.com%2Fxml%2Fmathml-extension%22%20height%3D%2228%22%20width%3D%2222%22%20wrs%3Abaseline%3D%2216%22%3E%3C!--MathML%3A%20%3Cmath%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F1998%2FMath%2FMathML%22%3E%3Cmsub%3E%3Cmi%3EV%3C%2Fmi%3E%3Cmn%3E2%3C%2Fmn%3E%3C%2Fmsub%3E%3C%2Fmath%3E--%3E%3Cdefs%3E%3Cstyle%20type%3D%22text%2Fcss%22%3Etext%7Bfill%3A%23000000%3B%7D%3C%2Fstyle%3E%3C%2Fdefs%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2218%22%20font-style%3D%22italic%22%20text-anchor%3D%22middle%22%20x%3D%226.5%22%20y%3D%2216%22%3EV%3C%2Ftext%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2213%22%20text-anchor%3D%22middle%22%20x%3D%2217.5%22%20y%3D%2224%22%3E2%3C%2Ftext%3E%3C%2Fsvg%3E) is the potential difference across resistor 2 in volts, V
        
- Recall that the e.m.f. of the power source will be equal to ![V subscript 1 space plus space V subscript 2](data:image/svg+xml;charset=utf8,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20xmlns%3Awrs%3D%22http%3A%2F%2Fwww.wiris.com%2Fxml%2Fmathml-extension%22%20height%3D%2228%22%20width%3D%2268%22%20wrs%3Abaseline%3D%2216%22%3E%3C!--MathML%3A%20%3Cmath%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F1998%2FMath%2FMathML%22%3E%3Cmsub%3E%3Cmi%3EV%3C%2Fmi%3E%3Cmn%3E1%3C%2Fmn%3E%3C%2Fmsub%3E%3Cmo%3E%26%23xA0%3B%3C%2Fmo%3E%3Cmo%3E%2B%3C%2Fmo%3E%3Cmo%3E%26%23xA0%3B%3C%2Fmo%3E%3Cmsub%3E%3Cmi%3EV%3C%2Fmi%3E%3Cmn%3E2%3C%2Fmn%3E%3C%2Fmsub%3E%3C%2Fmath%3E--%3E%3Cdefs%3E%3Cstyle%20type%3D%22text%2Fcss%22%3E%40font-face%7Bfont-family%3A'math117e62166fc8586dfa4d1bc0e17'%3Bsrc%3Aurl\(data%3Afont%2Ftruetype%3Bcharset%3Dutf-8%3Bbase64%2CAAEAAAAMAIAAAwBAT1MvMi7iBBMAAADMAAAATmNtYXDEvmKUAAABHAAAADRjdnQgDVUNBwAAAVAAAAA6Z2x5ZoPi2VsAAAGMAAAAoWhlYWQQC2qxAAACMAAAADZoaGVhCGsXSAAAAmgAAAAkaG10eE2rRkcAAAKMAAAACGxvY2EAHTwYAAAClAAAAAxtYXhwBT0FPgAAAqAAAAAgbmFtZaBxlY4AAALAAAABn3Bvc3QB9wD6AAAEYAAAACBwcmVwa1uragAABIAAAAAUAAADSwGQAAUAAAQABAAAAAAABAAEAAAAAAAAAQEAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACAgICAAAAAg1UADev96AAAD6ACWAAAAAAACAAEAAQAAABQAAwABAAAAFAAEACAAAAAEAAQAAQAAACv%2F%2FwAAACv%2F%2F%2F%2FWAAEAAAAAAAABVAMsAIABAABWACoCWAIeAQ4BLAIsAFoBgAKAAKAA1ACAAAAAAAAAACsAVQCAAKsA1QEAASsABwAAAAIAVQAAAwADqwADAAcAADMRIRElIREhVQKr%2FasCAP4AA6v8VVUDAAABAIAAVQLVAqsACwBJARiyDAEBFBMQsQAD9rEBBPWwCjyxAwX1sAg8sQUE9bAGPLENA%2BYAsQAAExCxAQbksQEBExCwBTyxAwTlsQsF9bAHPLEJBOUxMBMhETMRIRUhESMRIYABAFUBAP8AVf8AAasBAP8AVv8AAQAAAAAAAQAAAAEAANV4zkFfDzz1AAMEAP%2F%2F%2F%2F%2FWOhNz%2F%2F%2F%2F%2F9Y6E3MAAP8gBIADqwAAAAoAAgABAAAAAAABAAAD6P9qAAAXcAAA%2F7YEgAABAAAAAAAAAAAAAAAAAAAAAgNSAFUDVgCAAAAAAAAAACgAAAChAAEAAAACAF4ABQAAAAAAAgCABAAAAAAABAAA3gAAAAAAAAAVAQIAAAAAAAAAAQASAAAAAAAAAAAAAgAOABIAAAAAAAAAAwAwACAAAAAAAAAABAASAFAAAAAAAAAABQAWAGIAAAAAAAAABgAJAHgAAAAAAAAACAAcAIEAAQAAAAAAAQASAAAAAQAAAAAAAgAOABIAAQAAAAAAAwAwACAAAQAAAAAABAASAFAAAQAAAAAABQAWAGIAAQAAAAAABgAJAHgAAQAAAAAACAAcAIEAAwABBAkAAQASAAAAAwABBAkAAgAOABIAAwABBAkAAwAwACAAAwABBAkABAASAFAAAwABBAkABQAWAGIAAwABBAkABgAJAHgAAwABBAkACAAcAIEATQBhAHQAaAAgAEYAbwBuAHQAUgBlAGcAdQBsAGEAcgBNAGEAdABoAHMAIABGAG8AcgAgAE0AbwByAGUAIABNAGEAdABoACAARgBvAG4AdABNAGEAdABoACAARgBvAG4AdABWAGUAcgBzAGkAbwBuACAAMQAuADBNYXRoX0ZvbnQATQBhAHQAaABzACAARgBvAHIAIABNAG8AcgBlAAADAAAAAAAAAfQA%2BgAAAAAAAAAAAAAAAAAAAAAAAAAAuQcRAACNhRgAsgAAABUUE7EAAT8%3D\)format\('truetype'\)%3Bfont-weight%3Anormal%3Bfont-style%3Anormal%3B%7Dtext%7Bfill%3A%23000000%3B%3C%2Fstyle%3E%3C%2Fdefs%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2218%22%20font-style%3D%22italic%22%20text-anchor%3D%22middle%22%20x%3D%226.5%22%20y%3D%2216%22%3EV%3C%2Ftext%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2213%22%20text-anchor%3D%22middle%22%20x%3D%2217.5%22%20y%3D%2224%22%3E1%3C%2Ftext%3E%3Ctext%20font-family%3D%22math117e62166fc8586dfa4d1bc0e17%22%20font-size%3D%2216%22%20text-anchor%3D%22middle%22%20x%3D%2233.5%22%20y%3D%2216%22%3E%2B%3C%2Ftext%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2218%22%20font-style%3D%22italic%22%20text-anchor%3D%22middle%22%20x%3D%2252.5%22%20y%3D%2216%22%3EV%3C%2Ftext%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2213%22%20text-anchor%3D%22middle%22%20x%3D%2263.5%22%20y%3D%2224%22%3E2%3C%2Ftext%3E%3C%2Fsvg%3E)
    - ![[02_areas/PHYSICS/4/attachments/588bf336da98f80e5fa6d43cb5f426d4_MD5.jpg]]
---

### Types of circuit components

#### Power supplies

- Cells, batteries, power supplies and generators all **supply current** to the circuit
    

#### Resistors

- Potential dividers, fixed and variable resistors, thermistors and light-dependent resistors (LDRs) are all used to **control current**
    

#### Meters

- Ammeters and voltmeters are used to measure the current and potential difference
    
    - Ammeters are always connected in series whilst voltmeters are always connected in parallel
        

#### Switches and functional components

- Switches open and close a circuit and determine whether current can flow
    
- Functional components perform specific roles when current passes through them:
    
    - Motors rotate
        
    - Lamps emit light
        
    - Heaters transfer thermal energy
        
    - Bells emit a sound
        

#### Electromagnetic components

- Magnetising coils, relays and transformers use electromagnetic effects
    
    - Relays use a small current in one circuit to switch on a much larger current in another
        
    - Transformers 'step up' and 'step down' current and potential difference
        

#### Fuses

- Protect expensive components from current surges and act as a safety measure against fire
    

#### Thermistors

- A thermistor is a **non-ohmic** conductor and a temperature-dependent resistor
    
- The resistance of a thermistor changes depending on its **temperature**
    
    - As the temperature **increases** the resistance of a thermistor **decreases** and vice versa
    - ![[02_areas/PHYSICS/4/attachments/38e26eb29b48b44520f9e41313f9ea7f_MD5.jpg]]

#### Light-dependent resistors

- A light-dependent resistor (LDR) is a non-ohmic conductor and sensory resistor
    
- Its resistance automatically changes depending on the light energy falling onto it (illumination)
    
- As the **light intensity increases**, the **resistance** of an LDR **decreases**
- ![[02_areas/PHYSICS/4/attachments/7e22ea0188e956d219a9d5547047859d_MD5.jpg]]

## Diodes

- Diodes are occasionally drawn with a horizontal line running through the middle of them
    
- Diodes only allow current to flow through them in **one** direction (see the diagram below)
    
    - This is the direction that the triangle points in the diagram
- ![[02_areas/PHYSICS/4/attachments/a4e450981da2df3ab17863a21b97a6da_MD5.jpg]]
- _**When travelling in the same direction as the diode, current can flow. If the diode is flipped, it now prevents current from flowing in the circuit**_

- Light emitting diodes (LEDs) behave the exact same way, but they emit light when current flows through them




# Current in Circuits
A series circuit contains a **single** complete loop
- In a series circuit, the current is the **same value at any point**
    
    - This is because the number of electrons per second that passes through one part of the circuit is the same number that passes through any other part
        
- This means that **all** components in a closed-loop have the same current
![[02_areas/PHYSICS/4/attachments/eb443fc556f901ec5b2c3b168932e18a_MD5.jpg]]
![[02_areas/PHYSICS/4/attachments/ac8d82de4aebe3476ed0bcd1d08a6f81_MD5.jpg]]




A parallel circuit consists of multiple loops containing circuit components

### What is the rule for current in a parallel circuit?

- In a parallel circuit, the current **splits** along each **branch** at a junction
    
    - Some of it goes down one branch and the rest goes down the other
        
- This means that the current from the source is **larger** than the current in each branch
    

### Lighting circuits

- A lighting circuit is used to supply power to multiple light sources
    
    - Office lights are a common example, as multiple identical bulbs must have the same brightness
        
- Lighting circuits are constructed in **parallel** because:
    
    - Bulb's all have the same potential difference and therefore the same brightness
        
    - If one bulb breaks, the rest continue to function as current passes along each branch independently
        
    - This also means lamps can be switched off and on individually without breaking the whole circuit
The current **before** a junction is equal to the **sum** of currents along each branch **after** the junction

![[02_areas/PHYSICS/4/attachments/18c9c3bb8404bbd793b1b51f7084ea46_MD5.jpg]]

- At a **junction** in a **parallel** **circuit** (where two or more wires meet) the current is **conserved**
    
    - This means the amount of current flowing into the junction is equal to the amount of current flowing out of it
        
- This is because **charge** is conserved
    

- Note that the current does not always split equally – often there will be more current in some branches than in others
    
    - The current in each branch will only be identical if the **resistance** of the components along each branch are **identical**
        
- Current behaves in this way because it is the **flow of electrons**:
    
    - Electrons are physical matter – they cannot be created or destroyed
        
    - This means the total number of electrons (and hence current) going around a circuit must remain the same
        
    - When the electrons reach a junction, however, some of them will go one way and the rest will go the other
- ![[02_areas/PHYSICS/4/attachments/dae10d545dd1071fca2b85a83324b95a_MD5.jpg]]




## Resistors in series & parallel
- When two or more components are connected in **series**:
    
    - The **combined** resistance of the components is equal to the **sum** of individual resistances
![[02_areas/PHYSICS/4/attachments/c8d6273a1436a0d9c41e8015a1b561a3_MD5.jpg]]

- When resistors are connected in parallel, the **combined** resistance is **less than** the resistance of any of the individual components
    
- If two resistors of equal resistance are connected in parallel, then the combined resistance will halve
- To determine the combined resistance of any combination of two resistors, you must use the equation:
    

![1 over R space equals space 1 over R subscript 1 space plus space 1 over R subscript 2](data:image/svg+xml;charset=utf8,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20xmlns%3Awrs%3D%22http%3A%2F%2Fwww.wiris.com%2Fxml%2Fmathml-extension%22%20height%3D%2253%22%20width%3D%22128%22%20wrs%3Abaseline%3D%2230%22%3E%3C!--MathML%3A%20%3Cmath%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F1998%2FMath%2FMathML%22%3E%3Cmfrac%3E%3Cmn%3E1%3C%2Fmn%3E%3Cmi%3ER%3C%2Fmi%3E%3C%2Fmfrac%3E%3Cmo%3E%26%23xA0%3B%3C%2Fmo%3E%3Cmo%3E%3D%3C%2Fmo%3E%3Cmo%3E%26%23xA0%3B%3C%2Fmo%3E%3Cmfrac%3E%3Cmn%3E1%3C%2Fmn%3E%3Cmsub%3E%3Cmi%3ER%3C%2Fmi%3E%3Cmn%3E1%3C%2Fmn%3E%3C%2Fmsub%3E%3C%2Fmfrac%3E%3Cmo%3E%26%23xA0%3B%3C%2Fmo%3E%3Cmo%3E%2B%3C%2Fmo%3E%3Cmo%3E%26%23xA0%3B%3C%2Fmo%3E%3Cmfrac%3E%3Cmn%3E1%3C%2Fmn%3E%3Cmsub%3E%3Cmi%3ER%3C%2Fmi%3E%3Cmn%3E2%3C%2Fmn%3E%3C%2Fmsub%3E%3C%2Fmfrac%3E%3C%2Fmath%3E--%3E%3Cdefs%3E%3Cstyle%20type%3D%22text%2Fcss%22%3E%40font-face%7Bfont-family%3A'math1564b4c0e54101ac57a0cb68c16'%3Bsrc%3Aurl\(data%3Afont%2Ftruetype%3Bcharset%3Dutf-8%3Bbase64%2CAAEAAAAMAIAAAwBAT1MvMi7iBBMAAADMAAAATmNtYXDEvmKUAAABHAAAADxjdnQgDVUNBwAAAVgAAAA6Z2x5ZoPi2VsAAAGUAAABK2hlYWQQC2qxAAACwAAAADZoaGVhCGsXSAAAAvgAAAAkaG10eE2rRkcAAAMcAAAADGxvY2EAHTwYAAADKAAAABBtYXhwBT0FPgAAAzgAAAAgbmFtZaBxlY4AAANYAAABn3Bvc3QB9wD6AAAE%2BAAAACBwcmVwa1uragAABRgAAAAUAAADSwGQAAUAAAQABAAAAAAABAAEAAAAAAAAAQEAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACAgICAAAAAg1UADev96AAAD6ACWAAAAAAACAAEAAQAAABQAAwABAAAAFAAEACgAAAAGAAQAAQACACsAPf%2F%2FAAAAKwA9%2F%2F%2F%2F1v%2FFAAEAAAAAAAAAAAFUAywAgAEAAFYAKgJYAh4BDgEsAiwAWgGAAoAAoADUAIAAAAAAAAAAKwBVAIAAqwDVAQABKwAHAAAAAgBVAAADAAOrAAMABwAAMxEhESUhESFVAqv9qwIA%2FgADq%2FxVVQMAAAEAgABVAtUCqwALAEkBGLIMAQEUExCxAAP2sQEE9bAKPLEDBfWwCDyxBQT1sAY8sQ0D5gCxAAATELEBBuSxAQETELAFPLEDBOWxCwX1sAc8sQkE5TEwEyERMxEhFSERIxEhgAEAVQEA%2FwBV%2FwABqwEA%2FwBW%2FwABAAACAIAA6wLVAhUAAwAHAGUYAbAIELAG1LAGELAF1LAIELAB1LABELAA1LAGELAHPLAFELAEPLABELACPLAAELADPACwCBCwBtSwBhCwB9SwBxCwAdSwARCwAtSwBhCwBTywBxCwBDywARCwADywAhCwAzwxMBMhNSEdASE1gAJV%2FasCVQHAVdVVVQAAAQAAAAEAANV4zkFfDzz1AAMEAP%2F%2F%2F%2F%2FWOhNz%2F%2F%2F%2F%2F9Y6E3MAAP8gBIADqwAAAAoAAgABAAAAAAABAAAD6P9qAAAXcAAA%2F7YEgAABAAAAAAAAAAAAAAAAAAAAAwNSAFUDVgCAA1YAgAAAAAAAAAAoAAAAoQAAASsAAQAAAAMAXgAFAAAAAAACAIAEAAAAAAAEAADeAAAAAAAAABUBAgAAAAAAAAABABIAAAAAAAAAAAACAA4AEgAAAAAAAAADADAAIAAAAAAAAAAEABIAUAAAAAAAAAAFABYAYgAAAAAAAAAGAAkAeAAAAAAAAAAIABwAgQABAAAAAAABABIAAAABAAAAAAACAA4AEgABAAAAAAADADAAIAABAAAAAAAEABIAUAABAAAAAAAFABYAYgABAAAAAAAGAAkAeAABAAAAAAAIABwAgQADAAEECQABABIAAAADAAEECQACAA4AEgADAAEECQADADAAIAADAAEECQAEABIAUAADAAEECQAFABYAYgADAAEECQAGAAkAeAADAAEECQAIABwAgQBNAGEAdABoACAARgBvAG4AdABSAGUAZwB1AGwAYQByAE0AYQB0AGgAcwAgAEYAbwByACAATQBvAHIAZQAgAE0AYQB0AGgAIABGAG8AbgB0AE0AYQB0AGgAIABGAG8AbgB0AFYAZQByAHMAaQBvAG4AIAAxAC4AME1hdGhfRm9udABNAGEAdABoAHMAIABGAG8AcgAgAE0AbwByAGUAAAMAAAAAAAAB9AD6AAAAAAAAAAAAAAAAAAAAAAAAAAC5BxEAAI2FGACyAAAAFRQTsQABPw%3D%3D\)format\('truetype'\)%3Bfont-weight%3Anormal%3Bfont-style%3Anormal%3B%7Dtext%7Bfill%3A%23000000%3B%3C%2Fstyle%3E%3C%2Fdefs%3E%3Cline%20stroke%3D%22%23000000%22%20stroke-linecap%3D%22square%22%20stroke-width%3D%221%22%20x1%3D%222.5%22%20x2%3D%2218.5%22%20y1%3D%2223.5%22%20y2%3D%2223.5%22%2F%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2218%22%20text-anchor%3D%22middle%22%20x%3D%2210.5%22%20y%3D%2216%22%3E1%3C%2Ftext%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2218%22%20font-style%3D%22italic%22%20text-anchor%3D%22middle%22%20x%3D%2210.5%22%20y%3D%2241%22%3ER%3C%2Ftext%3E%3Ctext%20font-family%3D%22math1564b4c0e54101ac57a0cb68c16%22%20font-size%3D%2216%22%20text-anchor%3D%22middle%22%20x%3D%2233.5%22%20y%3D%2230%22%3E%3D%3C%2Ftext%3E%3Cline%20stroke%3D%22%23000000%22%20stroke-linecap%3D%22square%22%20stroke-width%3D%221%22%20x1%3D%2248.5%22%20x2%3D%2271.5%22%20y1%3D%2223.5%22%20y2%3D%2223.5%22%2F%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2218%22%20text-anchor%3D%22middle%22%20x%3D%2260.5%22%20y%3D%2216%22%3E1%3C%2Ftext%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2218%22%20font-style%3D%22italic%22%20text-anchor%3D%22middle%22%20x%3D%2256.5%22%20y%3D%2241%22%3ER%3C%2Ftext%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2213%22%20text-anchor%3D%22middle%22%20x%3D%2266.5%22%20y%3D%2249%22%3E1%3C%2Ftext%3E%3Ctext%20font-family%3D%22math1564b4c0e54101ac57a0cb68c16%22%20font-size%3D%2216%22%20text-anchor%3D%22middle%22%20x%3D%2286.5%22%20y%3D%2230%22%3E%2B%3C%2Ftext%3E%3Cline%20stroke%3D%22%23000000%22%20stroke-linecap%3D%22square%22%20stroke-width%3D%221%22%20x1%3D%22101.5%22%20x2%3D%22124.5%22%20y1%3D%2223.5%22%20y2%3D%2223.5%22%2F%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2218%22%20text-anchor%3D%22middle%22%20x%3D%22113.5%22%20y%3D%2216%22%3E1%3C%2Ftext%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2218%22%20font-style%3D%22italic%22%20text-anchor%3D%22middle%22%20x%3D%22109.5%22%20y%3D%2241%22%3ER%3C%2Ftext%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2213%22%20text-anchor%3D%22middle%22%20x%3D%22119.5%22%20y%3D%2249%22%3E2%3C%2Ftext%3E%3C%2Fsvg%3E)

- Where:
    
    - ![R](data:image/svg+xml;charset=utf8,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20xmlns%3Awrs%3D%22http%3A%2F%2Fwww.wiris.com%2Fxml%2Fmathml-extension%22%20height%3D%2222%22%20width%3D%2214%22%20wrs%3Abaseline%3D%2216%22%3E%3C!--MathML%3A%20%3Cmath%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F1998%2FMath%2FMathML%22%3E%3Cmi%3ER%3C%2Fmi%3E%3C%2Fmath%3E--%3E%3Cdefs%3E%3Cstyle%20type%3D%22text%2Fcss%22%3Etext%7Bfill%3A%23000000%3B%7D%3C%2Fstyle%3E%3C%2Fdefs%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2218%22%20font-style%3D%22italic%22%20text-anchor%3D%22middle%22%20x%3D%226.5%22%20y%3D%2216%22%3ER%3C%2Ftext%3E%3C%2Fsvg%3E) is the combined resistance in ohms, Ω
        
    - ![R subscript 1](data:image/svg+xml;charset=utf8,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20xmlns%3Awrs%3D%22http%3A%2F%2Fwww.wiris.com%2Fxml%2Fmathml-extension%22%20height%3D%2228%22%20width%3D%2221%22%20wrs%3Abaseline%3D%2216%22%3E%3C!--MathML%3A%20%3Cmath%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F1998%2FMath%2FMathML%22%3E%3Cmsub%3E%3Cmi%3ER%3C%2Fmi%3E%3Cmn%3E1%3C%2Fmn%3E%3C%2Fmsub%3E%3C%2Fmath%3E--%3E%3Cdefs%3E%3Cstyle%20type%3D%22text%2Fcss%22%3Etext%7Bfill%3A%23000000%3B%7D%3C%2Fstyle%3E%3C%2Fdefs%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2218%22%20font-style%3D%22italic%22%20text-anchor%3D%22middle%22%20x%3D%226.5%22%20y%3D%2216%22%3ER%3C%2Ftext%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2213%22%20text-anchor%3D%22middle%22%20x%3D%2216.5%22%20y%3D%2224%22%3E1%3C%2Ftext%3E%3C%2Fsvg%3E) is the resistance of resistor 1 in ohms, Ω
        
    - ![R subscript 2](data:image/svg+xml;charset=utf8,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20xmlns%3Awrs%3D%22http%3A%2F%2Fwww.wiris.com%2Fxml%2Fmathml-extension%22%20height%3D%2228%22%20width%3D%2221%22%20wrs%3Abaseline%3D%2216%22%3E%3C!--MathML%3A%20%3Cmath%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F1998%2FMath%2FMathML%22%3E%3Cmsub%3E%3Cmi%3ER%3C%2Fmi%3E%3Cmn%3E2%3C%2Fmn%3E%3C%2Fmsub%3E%3C%2Fmath%3E--%3E%3Cdefs%3E%3Cstyle%20type%3D%22text%2Fcss%22%3Etext%7Bfill%3A%23000000%3B%7D%3C%2Fstyle%3E%3C%2Fdefs%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2218%22%20font-style%3D%22italic%22%20text-anchor%3D%22middle%22%20x%3D%226.5%22%20y%3D%2216%22%3ER%3C%2Ftext%3E%3Ctext%20font-family%3D%22Times%20New%20Roman%22%20font-size%3D%2213%22%20text-anchor%3D%22middle%22%20x%3D%2216.5%22%20y%3D%2224%22%3E2%3C%2Ftext%3E%3C%2Fsvg%3E) is the resistance of resistor 2 in ohms, Ω
- ![[02_areas/PHYSICS/4/attachments/78714a2f3fe5d4f895482381ef49efcc_MD5.jpg]]



---

![[02_areas/PHYSICS/4/attachments/b59986f3aa4214ee73403929b67fddff_MD5.jpeg]]
![[02_areas/PHYSICS/4/attachments/24ad669feee9907a5df592f44a4b32fc_MD5.jpeg]]





