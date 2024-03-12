# MakeQRcode

Output qrcode by PowerShell for transmission data at some post-exploitation stage. 

## About

This PowerShell tool can be understood as follows:

> Native Windows Integration: The tool leverages PowerShell, which is a native scripting environment in the Windows operating system. This means there's no need for additional software installations to run the tool, assuming PowerShell is available and enabled on the system.

> Command-Line Execution: The tool is executed via the command line, which can be highly efficient for users comfortable with CLI environments. This allows for rapid execution of tasks without the need for a graphical user interface.

> No External Dependencies: The description suggests the tool does not require external dependencies, making it lightweight and easy to deploy, especially in environments where installing additional software is a concern due to security or administrative restrictions.

> Suitable for Post-Exploitation: The tool is designed for use in the post-exploitation phase of a cyber operation, which implies it's optimized for scenarios where stealth and efficiency are crucial. It can be used to exfiltrate data securely without attracting attention.

> Data Transmission via QR Code: By outputting data in the form of a QR code, the tool provides a novel way to transmit information discreetly. QR codes can be quickly scanned by mobile devices, facilitating easy data transfer without network connectivity.

> Versatility and Scriptability: As a PowerShell tool, it can be easily integrated into larger automation scripts or workflows, allowing for versatile use cases and the ability to chain together different post-exploitation tasks.

> Stealth Operations: Since the tool uses QR codes for data transmission, it may evade traditional data exfiltration detection methods that monitor network traffic, as the data transfer does not require network connectivity once the QR code is generated.

> Ease of Use: For users familiar with PowerShell, the tool should be straightforward to use, allowing them to generate QR codes from the command line with minimal effort.

## Sample

```
PS c:\> . .\makeqrcode.ps1

// output qrcode png file
PS c:\> Get-QRcode "path\to\you\text\file"

// print on the terminal
PS c:\> echo "you can text here to output on the terminal" | print-qrcode
```

Enjoy.
