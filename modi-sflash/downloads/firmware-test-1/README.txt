MODI SFlash Beta 2 - Firmware Test 1
Community test build / Wersja testowa dla społeczności
MODI13765 | 01.008.127 | 2026-11-10
Created by Modyfikator89 / ModyfikatorCasper

ENGLISH

This is a firmware compatibility test, not a claim that every firmware works.
Previous Beta 1 was tested on 13.60. This new binary needs console testing.
Keep your working Beta 1. This test uses a separate application title.

Requirements: an already working homebrew/jailbreak environment for your
firmware, a compatible elfldr listening locally on 9021, and ShadowMountPlus
or your existing working native-app mount setup. No Internet access is needed.
The app does not install or replace any jailbreak, loader or system patches.

1. Extract the ZIP. Put the .ffpkg in the same USB homebrew location you use
   for working MODI apps (normally /homebrew). Mount/refresh with ShadowMountPlus.
2. Connect a writable USB drive and open MODI SFlash Beta 2 - Firmware Test 1.
3. The readiness test starts automatically. It checks the loader and firmware;
   it does not read flash or kernel memory and does not change credentials.
4. Read the result. Unknown firmware shows UNSUPPORTED FIRMWARE and a log path.
   Repeat with Square on Backup, or Options > Test + USB report > X.
5. On the baseline 13.60 profile, close the result window and press X to back up.
   Other recognized pre-14.00 profiles are experimental: Options > Test backup
   is OFF by default. Enable it only if you are volunteering to test that profile.
   Firmware 14.x and unknown versions remain diagnostic-only in this build.
6. A readiness result is not a verified backup. Only BACKUP VERIFIED confirms
   two matching reads and verification of the stored USB files.

REPORTING RESULTS
Send the newest support_fwtest1_*.log from:
USB:/MODI_PS5_SFLASH_RO/diagnostics/
The window displays the actual file path. Include your console model, firmware,
loader/jailbreak/mounter names and versions, what you pressed and the result.
Report both successful and failed tests through the existing MODI project
support channel. Suggested subject: Firmware Test 1 / firmware / console model.
Do not send flash backups, drive keys or full console identifiers publicly.
There is no automatic upload. You choose which log to share.

If the USB drive is removed or unavailable, recent events remain in a bounded
RAM buffer while the app stays open. Reconnect USB; the app retries every two
seconds and creates a new report without overwriting old logs. Wait for the
saved-to-USB confirmation before closing. RAM is not persistent storage.
If the app cannot reach its UI at all, include a system error screenshot/report;
the app cannot log when the system has not allowed it to start.

Flash access is read-only. Files and logs are written to USB only. This app does
not program the physical chip or guarantee recovery from arbitrary damage.
Active Time/EMC data can be unavailable on some revisions; unavailable values
are not replaced with zero. Language and font are in Options (L1/R1 tabs).

POLSKI

To test zgodności firmware, nie deklaracja działania na każdej wersji systemu.
Poprzednia Beta 1 była testowana na 13.60. Nowa paczka wymaga testu na konsoli.
Zachowaj działającą Beta 1. Wersja testowa ma osobny identyfikator aplikacji.

Wymagany jest działający jailbreak/homebrew dla danego systemu, zgodny elfldr
na lokalnym porcie 9021 i ShadowMountPlus lub dotychczasowy sprawny mechanizm
montowania natywnej aplikacji. Internet nie jest potrzebny. Nie instalujemy
ani nie zmieniamy jailbreaka, loadera i poprawek systemowych.

1. Rozpakuj ZIP. Umieść .ffpkg w tym samym miejscu homebrew na USB co działające
   aplikacje MODI (zwykle /homebrew). Zamontuj/odśwież przez ShadowMountPlus.
2. Podłącz USB z możliwością zapisu. Uruchom aplikację Firmware Test 1.
3. Test gotowości uruchomi się automatycznie. Nie czyta Flash ani pamięci kernela
   i nie zmienia uprawnień procesu.
4. Przy braku profilu pojawi się „Nieobsługiwany firmware” oraz ścieżka raportu.
   Ponów kwadratem na ekranie Zrzut albo Opcje > Test + raport USB > X.
5. Dla bazowego 13.60 zamknij okno wyniku i naciśnij X, aby zrobić kopię.
   Inne rozpoznane profile poniżej 14.00 są eksperymentalne. Opcje > Backup testowy
   jest domyślnie wyłączony. Włącz go, jeśli świadomie zgłaszasz się do testu.
   14.x i nierozpoznane wersje pozostają tylko w trybie diagnostyki.
6. Wynik testu gotowości nie potwierdza backupu. Dopiero BACKUP ZWERYFIKOWANY
   oznacza dwa zgodne odczyty i sprawdzenie zapisanych plików z USB.

JAK ZGŁOSIĆ TEST
Prześlij najnowszy support_fwtest1_*.log z USB:/MODI_PS5_SFLASH_RO/diagnostics/.
Okno pokazuje dokładną ścieżkę. Dopisz model, firmware, nazwy i wersje jailbreaka,
loadera oraz montowania, co naciskałeś i co się wyświetliło. Przyjmujemy też logi
udanych testów. Użyj dotychczasowego kanału kontaktu projektu MODI.
Temat: Firmware Test 1 / firmware / model konsoli.
Nie udostępniaj publicznie dumpów Flash, kluczy ani pełnych identyfikatorów.
Log nie wysyła się sam. Wybierasz plik i przekazujesz go ręcznie.

Przy braku lub wypięciu USB ostatnie zdarzenia czekają w ograniczonym buforze RAM
do czasu zapisu, dopóki aplikacja jest otwarta. Włóż USB; ponowienie co 2 sekundy
tworzy nowy raport, bez nadpisywania poprzedniego. Zaczekaj na potwierdzenie zapisu.
Zamknięcie aplikacji przed zapisem traci RAM. Jeśli aplikacja w ogóle nie wchodzi
w UI, dołącz raport/zdjęcie błędu systemowego — nie mogła wtedy zapisać logu.

Źródło Flash jest tylko do odczytu. Pliki i logi trafiają wyłącznie na USB.
Aplikacja nie programuje kości i nie gwarantuje naprawy każdej awarii.
Active Time/EMC mogą być niedostępne na części rewizji; nie zastępujemy ich zerem.
Język i czcionka: Opcje, zakładki L1/R1.

Thanks to lewy20041 and the homebrew community / Dziękujemy scenie homebrew.
