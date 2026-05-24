# Android keyboard language packs

These files are intentionally outside `app/src/main/assets` so they are not
packaged into the base APK.

Upload this directory with its relative paths preserved to the endpoint used by
`YAPS_KEYBOARD_LANGUAGE_PACKS_BASE_URL`. The production default is:

```text
https://raw.githubusercontent.com/richawo/yaps-releases/main/android-keyboard-language-packs
```

then the German word list must be available at:

```text
https://raw.githubusercontent.com/richawo/yaps-releases/main/android-keyboard-language-packs/keyboard/nlp/de-DE/words.tsv
```

The app downloads the files into `filesDir/keyboard-language-packs/` using the
same relative paths, then the keyboard loaders read from device storage.
