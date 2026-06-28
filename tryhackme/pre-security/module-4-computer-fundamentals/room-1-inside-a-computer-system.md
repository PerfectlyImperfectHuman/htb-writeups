# Room: Inside a Computer System

**Module:** Module 4 — Comoputer Fundamentals
**Date completed:** June 28, 2026

## What this room covers

Before you try to secure a castle you need to learn about the layout of the castle, the different rooms, paths and people working there and once you have proper information about the castle only then can you truly make it secure just like that we are now learning about computers and it's componentes so that we can secure it in the future, we also learn about how a computer boots from pressing the power button to the Operating System starting

## Key concepts learned

- Computer — It is a device that does what it told to do but the great thing about it is that it can do complex tasks and hence is very useful in our daily lives

Components:

- Motherboard - it is basically the skeleton and nerves of the computer and it is the part that connects all the other parts together
- Central Processing Unit (CPU) or Processor - it is the brain of the computer and it does all the complex calculations and make all the decisions, it is connected to the motherboard using a CPU Socket
- Random Access Memory (RAM) - It is the short-term memory of the computer, it stores all the information that is frequently needed by the computer or the information that is useful for the task that is currently being performed and it is volatile which means that it loses all it's content once the power is lost
- Hard Disk Drives (HDD) & Solid State Drives (SSD) - They are the long-term memory of the computer and they store data for long-term (until it is deleted by the user or the drive is corrupted) and they are non-volatile which means that the content remains even after the power is lost. SSD's are better than HDD's as they don't have any moving parts (just chips) and are much faster than HDD's but they are more costly
- Network Adapter - It allows the computer to connect to other networks (like the internet) and they are mostly built-in to every computer but they can be added as Expansion cards, they usually connect with PCI Express Ports
- Power Supply Unit (PSU) - it is the heart of the computer it gives electricity to all the components, if it cna't provide enough electricity to the computer the system fails
- Graphics Card - This is the visual cortex of the computer it obtains information from the operating system or program being run and processes it into visual output for the user (the better the graphics the card, the better the visuals)
- Input/Output Devices - They are used to interact with the computer and to give input and obtain output from the computer ( just like our five senses ) Input Devices include: Keyboard, Mouse & Microphone etc while Output Devices include: Monitor, Speakers & Printers etc. They are connected through USB, HDMI and Display Ports

The Boot Sequence - How The Computer Boots/Starts:

- Pressing The Power Button - It all starts with the power button, you press it and it sends a signal to the PSU to allow power flow
- Firmware Starts (UEFI/BIOS) - It is the first program that runs and it initilizes and co-ordinates the components
- Power On Self Test (POST) - It is a test to check that all the compontents are receiving proper power flow and are working correctly. If there is some kind of error it starts beeping (Example: When you don't have RAM Installed the computer doesn't boot rather it starts beeping)
- Select Boot Device - Once it has been confirmed that all the components are working fine, the systems searchs for the Boot Up Routine, UEFI/BIOS has a priority list and it goes through that first to find the Boot Up Routine
- Initiate The Bootloader - When the boot loader routine has been found the system initiates the boot-loader. The Operating system is transferred from the Boot Device to the RAM and the computer boots/starts.

## Tools/commands used

- NONE

## Something that confused me at first

The Boot Sequence confused me a lot especially the term firmware (but I now understand that it means BIOS which I have always seen been used and UEFI is the newer version that has replaced BIOS)

Also this is the first time i have heard of a PCI Express Port but it is simply a type of port that allows you to connect Expansion Cards (Like Graphic Card or Network Adapter) into the PC and it has different types: x1 for sound cards, x4/x8 for ethernet or network adapters and x16 is the largest lane for Graphic Cards

## How this connects to real-world security

A lot of the times hackers tend to hack into the BIOS or UEFI ( the booting sequence ) hence knowing about this is useful in order to prevent that

## Next steps / what I want to explore more

I have always had a deep fascination about how computers work so this room was very fun for me and I truly want to learn more about the booting sequence and go deep into every single part of the motherboard and the other components
