Some odd testing results with this laptop. Testing done with Windows 11 24H2 (IoT LTSC), while plugged into AC power.

Using the ["HP" app (hidden, but accessible through Microsoft Store)](https://apps.microsoft.com/detail/9n9phdt62w94?hl=en-US&gl=US). System presets can be selected there.

**Performance Mode**

Run 1:
- MC 13992 pts
- SC 1599 pts

Thinking that somehow VT was the problem, I tried turning it off the BIOS... which also makes you lose all your passkeys apparently. Very annoying behavior.

Run 2 (Virtualization Disabled):
- MC 14412 pts
- SC 1635 pts

That's about a 2-3% improvement, but with the variation apparent in these CB results I think that I might've just gotten lucky on this run (still not up to part with online results). I tried other performance presets which seemed to engage the fan more.

After repasting the CPU with some aftermarket stuff (granted, on my unit, the factory paste was still pretty fresh and not crusty), I saw some differences. I also turned virtualization back on and to "default" settings.

Run 3 (After repaste):
- MC 14092 pts
- SC 1648 pts

**Smart Mode**

Run 1:
- MC 13625 pts
- SC 1604 pts

Now, after the thermal repaste, I tried the smart mode out of curiosity because it seems to engage the fans more. The results were a bit surprising:

Run 2 (After repaste):
- MC 14118 pts
- SC 1760 pts

This was much better than any result I've had before, both in MC and SC. It would seem that for this laptop the Smart Mode might actually be the best performance preset to use. Pretty unusual, but it works. The CPU will still reach 100C and throttle, but the wattage somehow remains more consistent now. The MC scores a tad bit low but overall seems like performance is as expected now.

**Balanced Mode**

Run 1: 
- MC 13725 pts
- SC 1599 pts

___

Results have too high of a variation of properly contextualize; this is inconsistent with testing done a year and some ago by benchmark sites. [NotebookCheck gets around 1708 SC and 15154 MC.](https://www.notebookcheck.net/Intel-Core-Ultra-7-155H-Processor-Benchmarks-and-Specs.783323.0.html) My machine has around a 5-7% deficit despite a clean install of the OS, the cause of which I can only assume is the CPU not being able to clock high enough.

Using HWInfo to monitor sensors, the processor is constantly pegged at 100C and is thermal throttling. Notably, however, the power limits seem to be working fine, the package power is stable around 20~30 W under SC loads and will stabilize around 45W for MC. 

Despite these loads, the fans hardly spin; the fan curve that comes on this laptop is very very limited. The fan will actually work harder in lower performance presets like "cool". 

GPU performance is frankly satisfactory for my use, especially for a mere 55 W part, and I did not feel the need to test it, as it performed how I expected it to in some games. If Nvidia's metrics are to be believed the GPU has no problem maintaining 55W load (while on AC power). On battery the power load fluctuates but is generally around 35-40 W.

I've reinstalled Windows around 4 times on this machine trying to figure it out, it is just too inconsistent.
