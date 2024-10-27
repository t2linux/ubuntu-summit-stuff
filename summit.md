# Opening

Good afternoon

Today we're talking about bringing Linux to modern Intel based Macs with T2 chips.

I'm Aditya, I maintain Ubuntu spinoff for T2 Macs
I'm Mark, I manage t2linux community
I'm Woohyun, I maintain some other distribution spinoffs


# What exactly is the T2 Security Chip? (Mark)
- T2 is a specialized security-focused SoC for Intel Macs
- Key functions:
  * Managing some USB devices (like keyboard, trackpad, Touch Bar and a camera)
  * Controls audio (speakers, and a microphone)
  * Manages NVMe SSD
  * Houses Secure Enclave for encryption
  * Handles video encoding/decoding

# Linux Challenge & Solution (Woohyun)
- Main obstacle: No T2 drivers meant no basic input device support nor access to the internal disk
- Breakthrough by Pawel Pawlowski:
  * First achieved NVMe SSD support (on Linux 5.4)
  * Developed critical apple-bce driver with three components:
    1. BCE: Basic T2 communication
    2. VHCI: Internal device support
    3. Audio support

# Project Progress (Aditya)
- Community effort led to t2linux project
- Current working features:
  * Internal disk access
  * Basic hybrid graphics
  * Full keyboard and trackpad support
  * Wi-Fi/Bluetooth (further improved by Asahi Linux collaboration)
  * FaceTime camera
  * Touch Bar
- Some features still have minor bugs but are overall usable

# Looking Ahead (Mark)
- Key goals:
  * Implement T2 SEP support for fingerprint reader
  * Fix suspending and resuming (which was broken recently by macOS Sonoma update)
- And there is challenge to find more kernel developers and hardware experts

# Current situation (Woohyun)
- We are maintaining spinoff versions of major Linux distributions:
  * Ubuntu, Linux Mint, Fedora
  * Arch Linux, EndeavourOS, NixOS
- There is also official upstream support in blendOS and CachyOS

# We need your help (Aditya)
- We are actively seeking kernel developers
- And looking to raise project awareness
- So thank you Canonical for the platform

# Demo (Mark)
If you want to see a demo of running Ubuntu on T2 based Intel MacBook Pro, then you can check it out
in Linux on Apple Hardware booth.

# Closing (Mark)
- Thank you for listening, if you have any questions we are happy to answer them.

*answer to all possible questions*

And again, if you want to see things working with your own eyes, or have more detailed questions, feel free to come by our booth.
