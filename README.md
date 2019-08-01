English | [简体中文](./README-CN.md)

# notepad-example-android
Example for notepad-android-sdk

# Usage
- Scan notepad
- Connect notepad
- Claim notepad
- Sync notepen pointer
- Import offline memo
- Get notepad info

## Scan notepad

```kotlin
val notepadScanner = NotepadScanner(context)
notepadScanner.callback = object : NotepadScanner.Callback {
    override fun onScanResult(result: NotepadScanResult) {
        println("onScanResult $result")
    }
}

notepadScanner.startScan()
// ...
notepadScanner.stopScan()
```