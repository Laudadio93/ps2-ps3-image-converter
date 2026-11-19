# PS2 & PS3 Image Converter

A standalone Windows application for converting PS2 Classics images and encrypting or decrypting supported PS3 disc ISOs. Select the system, operation, input, output, and matching key in the application, then follow the conversion progress.

**[Download the Windows application](https://github.com/Laudadio93/ps2-ps3-image-converter/releases/latest)** from the release assets. The executable includes its desktop runtime and conversion tools. Python and a separate toolkit installation are not required.

## Features

- Encrypt a PS2 DVD ISO into a PS2 Classics `ISO.BIN.ENC` file, or decrypt a supported PS2 Classics image into an ISO.
- Use the built-in PS2 CEX placeholder configuration or select a matching 16-byte klicensee for another supported PS2 Classics file.
- Encrypt or decrypt mapped regions of a PS3 disc ISO using its matching disc key.
- Accept PS3 disc keys as 16 raw bytes or 32 hexadecimal characters. The app checks for an identically named `.dkey` file beside a selected ISO.
- Browse for input, output, and key files. Conversions write to a separate output path.
- Follow live percentage progress, cancel a conversion, and see its completion or error message.
- Work locally once the application and your input files are available.

## Getting started

1. Download **PS2 and PS3 Encrypt Decrypt.exe** from the [latest release](https://github.com/Laudadio93/ps2-ps3-image-converter/releases/latest) and open it on 64-bit Windows.
2. Select **PS2** or **PS3** and choose encryption or decryption.
3. Browse to your source file and choose where to save the converted file.
4. Provide the matching key when the selected operation needs one. For PS3, the matching disc key is essential. A matching filename alone does not verify a key.
5. Start conversion and follow its progress. Check the resulting image against a trusted reference when available.

Use your own game images and applicable keys. The application requires enough free space for the output.

## Format details

| System | Input and output | Key and compatibility |
| --- | --- | --- |
| PS2 Classics | PS2 DVD ISO and PS2 Classics `ISO.BIN.ENC` | Supports the built-in CEX placeholder configuration and an applicable 16-byte klicensee. Encryption may add format padding and a footer. |
| PS3 disc image | Supported PS3 disc ISO with complete 2048-byte sectors and a supported region map | Requires the matching disc key. Automatic filename matching does not validate the key. IRD import is not part of this workflow. |

Successful conversion on the PC does not establish console compatibility or validate ownership of a key. Keep the source image and verify the output where possible.

## Credits

- The **ps3dev-net team** developed the ps2classic tool used for PS2 Classics image conversion. [PS2 Classics GUI by Aldo Vargas](https://www.psx-place.com/resources/ps2-classics-gui.638/)
- **SvenGDK** and contributors to OpenBurningSuite, **al3xtjames** and contributors to PS3Dec, and **Redrrx (Yacine S.)** and contributors to ps3dec provided PS3 disc-format and local-key lookup references. [OpenBurningSuite](https://github.com/SvenGDK/OpenBurningSuite) · [PS3Dec](https://github.com/al3xtjames/PS3Dec) · [ps3dec](https://github.com/Redrrx/ps3dec)
- **Microsoft and .NET contributors**, **Cygwin**, **zlib**, **OpenSSL contributors**, and the other developers identified in the app's About and license notices provide the underlying runtime and supporting tools. [Microsoft .NET](https://dotnet.microsoft.com/) · [Cygwin](https://www.cygwin.com/) · [zlib](https://zlib.net/) · [OpenSSL](https://openssl.org/)
- **Laudadio93** maintains the standalone application. PlayStation systems and marks belong to Sony Interactive Entertainment and their respective owners.

The executable also contains the PS4 engine resources inherited from the combined application, including emulator components and a PS4 packaging tool. Redistribution rights for those resources and the PS3 placeholder license have not been confirmed.

## Related project

The combined edition also includes PS3 and PS4 package studios and PS1 and PS2 memory-card tools. [All in One PS Classics Studio](https://github.com/Laudadio93/all-in-one-ps-classics-studio)
