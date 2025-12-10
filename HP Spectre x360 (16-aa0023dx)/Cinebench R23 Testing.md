Some odd testing results with this laptop. Testing done with Windows 11 24H2 (IoT LTSC), while plugged into AC power.

Using the ["HP" app (hidden, but accessible through Microsoft Store)](https://apps.microsoft.com/detail/9n9phdt62w94?hl=en-US&gl=US). System presets can be selected there.

**Performance Mode**

Run 1:
- MC 13992 pts
- SC 1599 pts

Run 2 (Virtualization Disabled):
- MC 14412 pts
- SC 1635 pts

**Smart Mode**

Run 1:
- MC 13625 pts
- SC 1604 pts

**Balanced Mode**

Run 1: 
- MC 13725 pts
- SC 1599 pts

___

Results have too high of a variation of properly contextualize; this is inconsistent with testing done a year and some ago by benchmark sites. NotebookCheck gets around 1708 SC and 15154 MC. My machine has around a 5-7% deficit despite a clean install of the OS.

Using HWInfo to monitor sensors, the processor is constantly pegged at 100C and is thermal throttling. Notably, however, the power limits seem to be working fine, the package power is stable around 20~30 W under SC loads and will stabilize around 45W for MC. 

Despite these loads, the fans hardly spin; the fan curve that comes on this laptop is very very limited. The fan will actually work harder in lower performance presets like "cool". 

GPU performance is frankly satisfactory for my use, especially for a mere 55W part, and I do not need to test it. If Nvidia's metrics are to be believed the GPU has no problem maintaining 55W load (while on AC power).

I've reinstalled Windows around 4 times on this machine trying to figure it out, it is just too inconsistent.
