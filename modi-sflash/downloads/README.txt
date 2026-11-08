MODI SFlash Beta 1
Created by Modyfikator89 / ModyfikatorCasper

Free homebrew for hobbyists and repair diagnostics.

Requirements
- A PS5 with an already working compatible homebrew setup.
- elfldr and ShadowMountPlus configured for native homebrew applications.
- A writable USB drive with enough free space.

Use
1. Copy MODI-SFlash-Beta-1.ffpkg to the USB homebrew folder used by your
   ShadowMountPlus setup.
2. Connect the USB drive to the PS5 and let ShadowMountPlus mount the app.
3. Launch MODI SFlash Beta 1 and press X.
4. Wait for VERIFIED before removing the USB drive.

The engine is embedded. No separate ELF or payload-folder copy is needed.

The application reads SFlash twice and saves the two files, SHA-256 checksums,
manifest and diagnostic logs to USB under MODI_PS5_SFLASH_RO. It reopens both
files and verifies the stored data. It does not write to the source flash.

Available console data may show Active Time, console information and recorded
EMC/thermal events. Unavailable readings remain unavailable. Recorded thermal
events are not a guarantee of the highest lifetime temperature.

Test status
The embedded engine is byte-for-byte identical to the engine that completed
a verified backup on one PS5 running firmware 13.60. The final Beta 1 frontend
uses a new font and has passed PC compilation/rendering checks; this exact
frontend has not yet been retested on a console. Other firmware and console
revisions are not confirmed.

The observed software reads were 2 MiB each. A verified read is not proof of
full physical NOR coverage or a tested programmer recovery/boot procedure.

Redistribution and component notices: see LICENSES.txt. No application source
or private console dumps/logs are included in this download.

Thanks to the homebrew community and all contributors.
Thanks to lewy20041 for introducing us to application development.
