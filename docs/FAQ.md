# FAQ

## Will Captura support Linux or Mac

Captura is written using .NET Framework, which at present, is supported only on Windows.

Software written using .NET Framework can work on Linux and Mac using Mono but the native calls and UI pose a problem to that.

Also, the recently released .Net Core only has support for console applications.

## Does Captura support DirectX Game Video Recording

Some newer games can be recorded using Desktop Duplication API.

Make sure to use a fast codec like Mp4 (x264).

A list of games that have been tried:

Game                                        | Status
--------------------------------------------|--------
NFS Most Wanted 2012                        | OK
Burnout Paradise Ultimate Box               | OK
Resident Evil 7                             | OK
Watch Dogs 2                                | FAIL

## Captura runs out of resources (high memory/CPU/disk usage) during recording

Atleast 2 GHz CPU and 4 GB RAM are recommended.

This may happen if frames are not being captured as fast as the framerate set.
Try a lower value of framerate, 15fps would always work.
We admit that the technology employed in Captura is not fast.

There are solutions like Fraps, Dxtory, OBS, and NVidia Share which provide 60fps recordings, but the technologies they use are complicated.

## Webcam capture does not work

Try updating the drivers from `Control Panel > Device Manager`.

## All options appear blank

This can occur due to Settings file being corrupted.

Try deleting `%AppData%/Captura` folder.