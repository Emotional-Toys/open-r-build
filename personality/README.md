## StikZap - CLIE tool for AIBO owners

StikZap is a CLIE program to check and fix certain types of AIBO memory sticks. StikZap tricks the (now defunct) Sony CLIE PDA to access the special pink sticks used by the (now defunct) Sony AIBO. NOTE: StikZap is a backup-like utility. It will save the necessary hardware stick information in a "Safety File" on the memory stick. It is intended for legal uses of making backup copies of software you own (and have legal licence to run). Don't make illegal copies of software.

### CLIE models supported

* Confirmed to work: all known CLIE models
* AFAIK all PalmOS4 and PalmOS5 devices will work with StikZap (NX, TJ, TH, UX, VZ, NZ, NR, SL and many others). The StikZap program may warn you about "guessing". You can ignore those warnings.
* The very old (monochrome) PalmOS3 models like the S300 will also work. After running the program, these older CLIEs may crash (there is a problem with the color icons). Simply reset the S300 CLIE and all will be well again
* Version 1.4 includes bug fix for PalmOS 4 devices. As always proceed at your own risk. Other PDAs won't work. It must be a CLIE (Sony Palm PDA) with a memory stick slot. 

### Sticks Detected

* Over 2 dozen common and not-so-common memory sticks.
* Includes 8MB and 16MB sticks, and the two different sizes of AiboMind sticks (32MB and 128MB). The Darker blue 128MB AiboMind3 stick also counts as a "pink" stick. 

### Sticks Repairable / Zap-able

* Any stick where you saved a _Safety File_, save it to the memory stick first, then save it to your computer.
* `PMS` _Programmable Memory sticks_ normally used for free programs like RCODE and Open-R SDK programs. Note `PMS` is a special kind of stick.
* AiboMind (1, 2 or 3) for ERS-7
* `PMS` and AiboMind are special cases for your convenience - they can be `zap`ed onto a stick even if you didn't bother to make a Safety File. In these two cases the physical sticks can run many different versions of software. As always, be sure the software you run is legally obtained.

### "Blank" Sticks that can be used as backups or as (blank) "PMS" sticks

* An official pink PMS stick (8MB or 16MB)
* Any old pink stick (for the ERS-2x0 or ERS-31x) that you don't use anymore (eg: the lame Party Mascot). Make a full backup first (with Safety File), then use it for something else.
* Any left-over 32MB AiboMind1/2 stick you don't use anymore (ie. after upgrading to Mind3)
* Any old light blue stick that works on the ERS-11x.
* Any light blue Sony "MSA-" stick of the right size (8MB -> 128MB: MSA-8, MSA-16, MSA-32, MSA-64, MSA-128)
* The pure white original Magic Gate sticks do work but they run slower than newer sticks. MS Pro sticks will _not_ work. Any stick larger than 128MB will _not_ work.
* Sony "MSH-" sticks may or may not work for you. Sony stopped making the "MSA-" sticks and now sells the "MSH-" ones. Some people report success (with MSH-128). Test them to see if they work for you.
* Non-Sony brand memory sticks may or may not work. Test them to see.
* The 32MB Black MS DUO stick that comes with the PSP will work, but you need a stick extender. Test it carefully first. The stick extender may get stuck in the CLIE or the AIBO!

### Warning

If you've never used a stick reader before, or backed up your memory stick before, you shouldn't be using StikZap. StikZap is not that difficult or risky, but if it is the first time you've attempted stick backups, you may screw it up. Improper use of StikZap (without making a proper backup first) can screw up your memory sticks. Become familiar with more general uses of a SONY BRAND stick reader before continuing. This tutorial assumes you are generally familiar with using a CLIE (installing and running programs). You should also be familar with backing up your memory stick contents to your computer (using a Sony brand stick reader or your CLIE in MSImport/DataImport mode).

## Installation

* Backup your PDA first. Hotsync is usually sufficient.
* TIP: Soft reset before you start. Not strictly necessary, but helpful when trying a new program for the first time.
* Download the program [StikZap_14.prc](/personality/StikZap_14.prc).
* Install the .prc file on your CLIE, using HotSync or copying to stick. If you don't know how to do this, go read the "Warning".
* The program "StikZap" should appear in your program launcher. Don't run it right now, especially if there is no memory stick in the CLIE.
* Only use a Sony Brand memory stick reader. Your CLIE running in "MSImport" or "DataImport" mode is safe too - connected to your PC with the USB cable.

### Using the program - common operations

* Proceed at your own risk. StikZap can be used to fix your damaged sticks. When used improperly, it can break your working sticks.
* First insert the memory stick into your CLIE. The CLIE will usually beep. Sometimes the CLIE launcher will show you the programs on the stick (in this case none).
* Run the "StikZap" program on your CLIE, it will tell you what to do. See below for common scenarios.
* When done, remove the memory stick from the CLIE
* If appropriate put the stick in your AIBO and test it.
* NOTE: Be sure the memory stick is not write protected (switch on back should not show red)
* NOTE: the CLIE will usually create a "PALM" folder at the top level of the memory stick (with Launcher and PROGRAMS folders inside). You can ignore it. 

### Common Case : Backup your sticks

This is the most common case. You should do this before playing around with the contents of your stick. NOTE: In general there is no need to backup a "PMS" programmable stick

* First insert the memory stick into your CLIE. The CLIE will usually beep.
* Run the "StikZap" program on your CLIE. It will Check the stick for you.
* The first time it is run, StikZap should recommend "Create Safety, then copy entire stick to PC"
* Press the "Create Safety" button, then press "OK"
* You are done with StikZap. You must backup the entire memory stick to your PC for your own safety.

* Option One (doing it on the CLIE):
    - Exit StikZap.
    - Run the MSImport or DataImport program on the CLIE.
    - Plug in the CLIE (or CLIE in a cradle) to your PC with the USB cable
    - The CLIE's memory stick will appear as a new drive on "My Computer" (if it doesn't you may need to install the CLIE drivers on your PC)
    - Drag the files in that drive to your Desktop, or use a program like WinZip to create a backup copy of the entire stick contents. 

* Option Two (using a separate, Sony Brand, stick reader)
    - Remove the memory stick from the CLIE (the StikZap program will exit)
    - Insert the memory stick in your separate, Sony Brand, stick reader attached to your PC.
    - Drag the files from the memory stick drive to your Desktop, or use a program like WinZip to create a backup copy of the entire stick contents. 

The backup is your personal backup of your stick. Keep it safe. It includes information about your stick hardware, the software (copyrighted by Sony and others), personal information about your AIBO, as well as any custom personality your robot has developed.

### Common Case : Stick gets corrupted / Restore it

* If your stick is corrupted at a low level, you may need to format it first (tutorial to be written)
* Place the corrupted stick into your stick reader (or if using your CLIE as a stick reader, run the MSImport/DataImport program)
* Using your PC, select all the files and folders on the memory stick and delete them. If necessary, empty the Recycling Bin.
* Restore the backup you made earlier to the memory stick. This must be a backup you made after the "Create Safety" step described above.
* There should be an "OPEN-R" folder at the topmost folder of the memory stick. There may be others ("CUSTOM", "PALM" etc)
* Remove the stick from the memory stick reader and place it in the CLIE. If using the CLIE as a memory stick reader, stop and exit MSImport/DataImport.
* Run the "StikZap" program on your CLIE. It will Check the stick for you.
* It should automatically recommend "Press 'Use Safety', (only if you kept a backup)"
* Press the "Use Safety" button, and pick "Yes"
* Remove the stick from your CLIE, and place in AIBO. Boot AIBO and see if it works.
* If it fails to boot, the stick may have lower level formatting problems, or may not work as an AIBO stick. 

ome websites have "Virgin" memory stick images of various commercial AiboWare programs. These won't work for this purpose.

### Common Case : Make a working backup (stick copy)

Start with a stick you aren't using. If an AIBO stick, make a backup with the safety file (see above) and save it away somewhere on your PC. See above for other kinds of "blank" sticks you can use (ie. old pink stick, or old light blue sticks). Then follow the instructions above for restoring a corrupted stick. Some websites have "Virgin" memory stick images of various commercial AiboWare programs. These won't work for this purpose either.

### Common Case: Make your own "PMS" stick
Start with a stick you aren't using. If an AIBO stick, make a backup with the safety file (see above) and save it away somewhere on your PC. See above for other kinds of "blank" sticks you can use (ie. old pink stick, or old light blue sticks). After you have a good backup, you can `ZAP` it to make it a blank PMS stick.

* If you care what was on the stick before, be sure you have a backup (see above)
* Insert the memory stick into your CLIE. The CLIE will usually beep.
* Run the "StikZap" program on your CLIE. It will Check the stick for you. You can ignore the recommendations.
* From the menu, pick "ZAP PMS". Answer "Yes" and your stick will now be a PMS stick.
* Using a stick reader (or the CLIE in MSImport/DataImport mode), delete any old files and install a PMS personality and see if it works.
* Suggestions: (especially for testing the first time)
    - For the ERS-210/210A - RCodePlus 2.52A (210)
    - For the ERS-220/220A - RCodePlus 2.52A (220)
    - For the ERS-311/312/31L - RCodePlus 2.52A (31x)
    - For the ERS-7 - RCODE7_YART703_E.zip 
* Remove the stick from the stick reader (or CLIE) and put it in AIBO.
* Boot AIBO, and see if it stretches and sit up.
* If it fails to boot or doesn't stretch the stick you tried may not work in AIBO (or may have format problems).
* If there is a problem AIBO usually shut downs early in the boot process. If the stick stays locked for more than 2 or 3 minutes, then eject the stick using the leg tool. 

### Special Case : untested CPU

It has been tested on a small number of models, but StikZap is smart and will guess where necessary. If you test it on a newer model, it will tell you it is guessing. If the guess works, please email me with the results of the menu command `Guess Cpu` If it fails, please run the menu command `Save Cpu` with an (8 or 16MB) Aibo memory stick in the CLIE. It will create a file on the stick called `INTERNAL.BIN`. This file is the basis for future building-upon the platform.