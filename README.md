# DymoTeaLabel
Webform to quickly generate Dymo Label Printer files (and print them) for tea caddys

You'll need full **Dymo Label** software installed on Windows or macOS and **DYMO.DLS.Printing.Host.exe** running (should be by default).

![Demo](demo.png)

## Templates - adding new one
1. Dump template from *Dymo Label* and save in location accessible to directory with html
2. Add new filename to `select` with id `templateFile` 
3. Use following template tokens in XML/`.label` file - they are simply replaced with values from form:
   - `teaName`
   - `brTemp` (brewing temp)
   - `brTime` (brewing time)
   - `teaType`
   - `info1` (top line)
   - `info2` (bottom line)
   - `TOKEN_URL` (URL)
