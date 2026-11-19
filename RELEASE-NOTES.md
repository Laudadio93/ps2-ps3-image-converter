# First standalone release

This release provides the PS2 and PS3 image conversion workflow from All in One PS Classics Studio as a standalone Windows executable. It includes the electric-blue disc and padlock icon and opens directly to the conversion interface.

## Included capabilities

- Encrypt PS2 DVD ISOs into PS2 Classics images and decrypt supported PS2 Classics images back to ISO.
- Use the built-in PS2 CEX placeholder configuration or select a matching 16-byte klicensee.
- Encrypt and decrypt the mapped regions of supported PS3 disc ISOs using a matching disc key.
- Detect a same-named PS3 `.dkey` file, with support for raw 16-byte or hexadecimal 32-character keys.
- Choose separate source and destination paths, view progress, cancel a job, and receive completion or error messages.
- Use the application offline after downloading it. The executable carries its Windows runtime and conversion resources.

Select the appropriate system and operation, supply your own input and matching key, and choose an output location with sufficient free space. The PS3 workflow requires a supported region map and complete 2048-byte sectors. An identified key filename does not confirm that its contents match the disc. IRD import is not supported.

The standalone application was rebuilt from the combined edition. Its Windows icon includes eight sizes. Conversion results should be checked against a trusted reference where possible.

The executable also contains PS4 emulator and package tool resources inherited from the combined application. Redistribution rights for those resources and the PS3 placeholder license have not been confirmed.

Credits and further details are available in the [project README](https://github.com/Laudadio93/ps2-ps3-image-converter#readme).
