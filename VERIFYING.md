# Checking the download

If you want to make sure the download is complete, compare its SHA-256 with the values published here. A matching hash means the bytes match. It isn't a virus scan or a replacement for checking where you got the files.

Put `SHA256SUMS.txt` in the same folder as the downloaded files. Open PowerShell in that folder and run:

```powershell
Get-Content -LiteralPath .\SHA256SUMS.txt | ForEach-Object {
    $expected, $name = $_ -split '  ', 2
    if (Test-Path -LiteralPath $name -PathType Leaf) {
        $actual = (Get-FileHash -LiteralPath $name -Algorithm SHA256).Hash
        if ($actual -ieq $expected) { "OK: $name" } else { "MISMATCH: $name" }
    } else { "Not downloaded: $name" }
}
```

Each file you downloaded should say **OK**. You can skip the separate dependency sources if you only want to use the app; its entry will say **Not downloaded**. All four app parts are required.

If a file says **MISMATCH**, download it again before extracting or running anything. Compare the manifest itself with a trusted copy from this release page.

## Complete app ZIP

If you joined the four parts into one ZIP, run:

```powershell
(Get-FileHash -LiteralPath '.\Desolated-Transcriptor-1.4.0-Windows-x64.zip' -Algorithm SHA256).Hash -ieq '2bc053fb17f5b5b5c0edf9efa3b595ba352b4f4f20cc8512afa8345b075b7d5f'
```

It should return **True**. This is the same verified release ZIP; splitting and joining it doesn't change its contents.

## Files inside the app

The extracted app has another `SHA256SUMS.txt` in its parent folder. Run the first command from that folder to check the packaged files. That manifest covers the original app files; settings, sessions, exports & cache files created later aren't part of the clean release.
