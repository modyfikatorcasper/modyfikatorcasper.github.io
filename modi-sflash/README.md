# MODI SFlash Beta 1

![MODI SFlash](assets/cover.png)

Free PS5 homebrew for hobbyists and repair diagnostics. Back up the console-exposed SFlash image to USB, verify two saved copies, and view available Active Time and recorded EMC/thermal events.

**[Download Beta 1](downloads/MODI-SFlash-Beta-1.zip)** · **[Project page](https://modyfikatorcasper.github.io/modi-sflash/)** · [Checksums](downloads/SHA256SUMS.txt)

## Start in four steps

1. Extract the ZIP and put `MODI-SFlash-Beta-1.ffpkg` in the USB `homebrew` folder used by your ShadowMountPlus setup.
2. Start your already configured PS5 homebrew environment with **elfldr**, let **ShadowMountPlus** mount the application, and open its tile.
3. Keep the USB drive connected and press **X**.
4. Wait for **VERIFIED** before removing the USB drive. Find the two copies, SHA-256 checksums, manifest and logs under `MODI_PS5_SFLASH_RO` on USB.

The engine is embedded in the application. **No separate ELF or payload-folder copy is needed.**

## What the app shows

- **Two verified copies:** independent reads, saved-file comparison and SHA-256 verification after closing and reopening the USB files. The source flash is opened read-only.
- **Active Time:** available recorded console operating time, displayed in days, hours, minutes and seconds. This is operating time, not a game-play counter.
- **EMC history:** available recorded temperatures and error events, with an expanded details window.
- **Console information:** available model, drive, storage and firmware information; identifiers are masked by default.
- **Options:** automatic language selection, manual PL/EN selection and two text styles.

![Backup results — PC preview with sample values](assets/results.png)

![Console information — PC preview with sample values](assets/console-info.png)

The images are PC-rendered previews with clearly marked sample data, including sample thermal events. They are not measurements from an additional console.

## Beta test scope

The embedded engine is byte-for-byte identical to the engine that completed a verified backup on **one PS5 running 13.60**. Both stored copies were 2 MiB and matched. The final Beta 1 frontend has passed PC compilation and rendering checks; this exact frontend is not yet retested on a console. Other firmware and hardware revisions are not confirmed. PS5 Pro testing is pending.

Unavailable readings remain unavailable. Recorded thermal events are not a guarantee of the highest lifetime temperature and do not diagnose a cooling fault on their own.

The app copies the SFlash image exposed by the console. A verified software read is not proof of full physical NOR coverage or a tested chip-programmer recovery procedure.

## Credits and notices

Created by **Modyfikator89 / ModyfikatorCasper**.

Thanks to the **PS5 homebrew community**, all contributors, and **lewy20041** for introducing us to application development.

The application is free to download. Redistribution terms and required component notices are in [LICENSES.txt](downloads/LICENSES.txt). The download contains the application, instructions, licenses and checksums; it contains no private console data or application source.
