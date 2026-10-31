# Getting the app running

The app is a big download because the engines, models & runtimes are already in it. You don't need to install Python or Shotcut, make an account, or download models when you start it.

GitHub limits each release file to under 2 GiB, so the app ZIP comes in four parts. You need all four.

1. Download `Desolated-Transcriptor-1.4.0-Windows-x64.zip.001`, `.002`, `.003` & `.004` from [the release](https://github.com/datwhiteguy/Desolated-Waves-Transcriptor/releases/tag/v1.4.0). Put them together in one folder. Keep their names as they are.
2. Check the parts against `SHA256SUMS.txt` if you want to verify the download. [The checksum steps are here](VERIFYING.md).
3. With a current version of [7-Zip](https://www.7-zip.org/), open the `.zip.001` file and extract the complete archive. It reads the other three parts from the same folder.
4. Keep **Desolated Waves's Transcriptor** together in a writable folder. Open **Desolated Transcriptor.exe**.
5. Open [User Guide.pdf](https://github.com/datwhiteguy/Desolated-Waves-Transcriptor/releases/download/v1.4.0/User-Guide.pdf) for the settings, review tools & export steps. The same guide is inside the app folder.

You need Windows 10 or 11, a 64-bit AVX2-capable processor & enough free space. The download is about 7.62 GB and the extracted app is about 10.76 GB. Leave extra space for temporary audio and your exports. Keep the app out of protected folders where it can't save its files.

## Want a normal ZIP instead?

Open **Command Prompt** in the folder holding the four parts. Make sure `Desolated-Transcriptor-1.4.0-Windows-x64.zip` doesn't already exist there, then run this one command:

```bat
copy /b "Desolated-Transcriptor-1.4.0-Windows-x64.zip.001"+"Desolated-Transcriptor-1.4.0-Windows-x64.zip.002"+"Desolated-Transcriptor-1.4.0-Windows-x64.zip.003"+"Desolated-Transcriptor-1.4.0-Windows-x64.zip.004" "Desolated-Transcriptor-1.4.0-Windows-x64.zip"
```

That puts the original ZIP back together. It needs another 7.62 GB of free space. Its SHA-256 must be:

```text
2bc053fb17f5b5b5c0edf9efa3b595ba352b4f4f20cc8512afa8345b075b7d5f
```

You can then extract the complete ZIP with Windows or 7-Zip. Don't try to run the app from inside the archive.

## Which other downloads do I need?

- **User-Guide.pdf:** the manual, including what the engine settings do.
- **SHA256SUMS.txt:** checksums for the download parts & companion files.
- **Desolated-Transcriptor-1.4.0-Windows-x64.zip.sha256:** checksum for the complete ZIP after joining the parts.
- **Desolated-Transcriptor-1.4.0-Third-party-sources.zip:** source files for the bundled third-party dependencies. You don't need this to run the app. Keep it available beside the app if you redistribute this release.
- **Desolated-Transcriptor-1.4.0-Third-party-sources.zip.sha256:** checksum for that dependency archive.

GitHub also adds buttons named **Source code (zip)** & **Source code (tar.gz)**. Those contain the documentation in this repository. They aren't the app download, and they don't contain Desolated Transcriptor's application source.
