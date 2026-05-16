# downloaded_video.mp4 parts

The original `downloaded_video.mp4` was split into six binary parts, each under 100 MB.

To reconstruct it on Linux/macOS:

```bash
cat downloaded_video.mp4.part_* > downloaded_video.mp4
sha256sum -c downloaded_video.mp4.sha256
```

On Windows PowerShell:

```powershell
cmd /c copy /b downloaded_video.mp4.part_00+downloaded_video.mp4.part_01+downloaded_video.mp4.part_02+downloaded_video.mp4.part_03+downloaded_video.mp4.part_04+downloaded_video.mp4.part_05 downloaded_video.mp4
```
