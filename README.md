# nullos

debian-based security-focused linux distro.

## status

**v1.0-alpha** - first working build. rough around the edges.

## what's in it

- debian 13 (trixie) base
- kde plasma desktop
- security toolkit (nmap, wireshark, hashcat, john, hydra, aircrack-ng, masscan, nikto, sqlmap)
- dev environment (vscode, gcc, g++, python3, git, cmake)
- brave browser, firefox
- performance tweaks (zram, preload, optimized sysctl, I'm all for a be)

## known issues

- spotify repo broken during build (install manually: `sudo snap install spotify` or wait for v1.1)
- no custom theming yet (coming soon)
- no NullOS control center (planned for v1.0-final)
- based on debian testing (trixie) - occasional package updates may cause instability


## download

**[download nullos v1.0-alpha (5.16 GB)](https://archive.org/details/nullos-1.0-alpha-amd64)**

md5: `f9e96b7b97f6709ab713a6ff993e6fd7` (will be updated to SHA soon, but for now it is md5)

### verify download
```bash
md5sum nullos-1.0-alpha-amd64.iso
```

### create bootable usb
```bash
# linux
sudo dd if=nullos-1.0-alpha-amd64.iso of=/dev/sdX bs=4M status=progress && sync

# or use balena etcher (recommended for beginners)
```

## roadmap

### v1.0-final
- Hopefully good security and security tools
- custom glassmorphism theme
- nullos control center dashboard
- proper installer (calamares)
- boot screen branding

### v1.1+
- spotify integration
- custom desktop widgets
- arm64 support (raspberry pi or anything alike)
- advanced first-boot wizard

## building from source

used [cubic](https://github.com/PJ-Singh-001/Cubic) for v1.0-alpha. 

base: debian 13 kde live iso

will switch to live-build for reproducible builds in v1.0-final.

## requirements

- x86_64 (amd64) processor
- 4gb ram minimum (8gb recommended)
- 25gb free disk space

## why nullos?

wanted a daily driver that doesn't compromise on security tools like Kali. kali is great for pentesting but not for everyday use. ubuntu is solid but lacks pre-configured security stuff. nullos is the middle ground.

also learning distro dev in public. expect mistakes from me lol.

## contributing

not ready for contributions yet. once v1.0-final drops and the build process is documented, i'll open it up.

## disclaimer

**this is an alpha release.** do not use in production environments without applying security updates first. intended for testing, learning, and development.

## license
[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
Apache 2.0

---

built by [@madis-o](https://github.com/madis-o) | nullsec
