# Analog Clock — Android (Kotlin)

ಹೋಮ್ ಸ್ಕ್ರೀನ್ widget ಮತ್ತು ಲಾಕ್-ಸ್ಕ್ರೀನ್ ಶೈಲಿಯ full-screen clock. ಪ್ರತಿಯೊಂದಕ್ಕೂ ಪ್ರತ್ಯೇಕ ಸೆಟ್ಟಿಂಗ್ಸ್.

## ಫೀಚರ್
- 8 clock designs: Classic, Minimal, Roman, Neon, Modern, Pastel, Bold, Dots
- 8 colour themes: Ocean, Sunset, Forest, Lavender, Mono, Neon, Gold, Candy
- Toggles: ಸೆಕೆಂಡ್ ಮುಳ್ಳು, ದಿನಾಂಕ, ಅಂಕಿಗಳು, ಕಪ್ಪು ಹಿನ್ನೆಲೆ
- Home ಮತ್ತು Lock ಗೆ ಪ್ರತ್ಯೇಕ settings
- Live preview ಮತ್ತು grid view ಆಯ್ಕೆ
- ಆಫ್‌ಲೈನ್ — ಯಾವುದೇ ಇಂಟರ್ನೆಟ್ ಅಥವಾ ಬಾಹ್ಯ ಲೈಬ್ರರಿ ಇಲ್ಲ

## ತೆರೆಯುವುದು
Android Studio → Open → `AnalogClock` ಫೋಲ್ಡರ್ → Run ▶ (min SDK 26, target SDK 35)

## ಮಿತಿಗಳು
- Android third-party apps ಅನ್ನು ನೈಜ lock screen ನಲ್ಲಿ widget ಆಗಿ ಇರಿಸಲು ಅನುಮತಿಸುವುದಿಲ್ಲ. "Lock-screen clock" ಬಟನ್ lock ಆದ ಮೇಲೆಯೂ full-screen ತೋರಿಸುತ್ತದೆ.
- Widget ನಿಮಿಷಕ್ಕೊಮ್ಮೆ ನವೀಕರಣಗೊಳ್ಳುತ್ತದೆ (ಸೆಕೆಂಡ್ ಮುಳ್ಳು widget ನಲ್ಲಿ ಇಲ್ಲ).

## ಲ್ಯಾಪ್‌ಟಾಪ್ ಇಲ್ಲದೆ APK ಪಡೆಯುವುದು (GitHub Actions)
1. GitHub ನಲ್ಲಿ ಹೊಸ repository ಮಾಡಿ (ಉದಾ: `analog-clock`), ಅದನ್ನು Public ಅಥವಾ Private ಇಡಬಹುದು.
2. `AnalogClock` ಫೋಲ್ಡರ್ **ಒಳಗಿನ** ಎಲ್ಲಾ ಫೈಲ್‌ಗಳನ್ನು (`.github` ಸೇರಿ) repository ಯ ಮೇಲ್ಭಾಗಕ್ಕೆ upload ಮಾಡಿ.
3. Repository ನಲ್ಲಿ **Actions** ಟ್ಯಾಬ್ → "Build APK" → **Run workflow** ಒತ್ತಿ (ಅಥವಾ upload ಆದ ತಕ್ಷಣ ತನ್ನಿಂದ ಆರಂಭವಾಗುತ್ತದೆ).
4. ಕೆಲವು ನಿಮಿಷಗಳ ನಂತರ run ಮುಗಿದ ಪುಟದ ಕೆಳಗೆ **AnalogClock-debug-apk** artifact ಕಾಣುತ್ತದೆ. ಅದನ್ನು ಡೌನ್‌ಲೋಡ್ ಮಾಡಿ (ZIP ಒಳಗೆ `app-debug.apk`).
5. ಫೋನ್‌ನಲ್ಲಿ APK ತೆರೆದು ಇನ್‌ಸ್ಟಾಲ್ ಮಾಡಿ. "Unknown apps" ಅನುಮತಿ ಕೇಳಿದರೆ ನಿಮ್ಮ ಬ್ರೌಸರ್/ಫೈಲ್ ಮ್ಯಾನೇಜರ್‌ಗೆ ಅನುಮತಿ ನೀಡಿ.
