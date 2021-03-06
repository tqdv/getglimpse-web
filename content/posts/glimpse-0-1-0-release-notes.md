---
title: "Glimpse 0.1.0 Release Notes"
date: 2019-11-22T12:16:00+00:00
draft: false
---
This is the very first binary release for Glimpse Image Editor. The primary objective was to complete the re-brand, remove obvious distractions from the user interface, learn the various technologies involved and lay the groundwork for future development.

This project was started on Friday 5th July 2019 by a small group of [fediverse](https://en.wikipedia.org/wiki/Fediverse) users who had never even set eyes on the upstream code before. Over the last four months we have been overwhelmed by the support we have received from over 1000 social media followers across [Twitter](https://twitter.com/glimpse_editor) and [Mastodon](https://bobadon.co.uk/@glimpse), dozens of financial backers across Patreon and [Open Collective](https://opencollective.com/glimpse), and over 100 people who have joined [our public Matrix channel](https://glimpse-editor.org/about/[#glimpse:matrix.org](https://matrix.to/#/#glimpse:matrix.org)) to volunteer their expertise and ensure we make good decisions. We would like to thank everyone that helped us achieve our objectives, and we hope we can keep the momentum going as we start to plan what comes next in Glimpse 0.2.0.

We are also pleased to announce that in October 2019 we [donated $50 to the GNU Image Manipulation Program](https://opencollective.com/glimpse/expenses/10167) as part of our commitment to share a portion of the donations we receive for each new release with them. We hope in future this amount will increase and be augmented with new bug fixes and features from our own contributors.

## Installation
GNU/Linux users can install Glimpse 0.1.0 as a Flatpak from the Flathub repository. There are also a number of additional installation options for Linux detailed on our [Downloads](/downloads/) page.

Windows users can use an MSI file to install Glimpse 0.1.0 on 32-bit and 64-bit systems running Windows 7 or later. We chose that type of installer to assist businesses and schools using centralised software management systems. This can also be found on the [Downloads](/downloads/) page.

## Known Issues
* We do not support MacOS at this time
* The current Windows installer triggers security warnings because it has not been signed. We intend to provide a signed installer very soon
* There is no native 64-bit installer for Windows (use the 32-bit one instead)
* Man pages in the terminal have not been updated
* Compatibility with upstream offline help pages has not been tested
* Some translations may still need updating

## New Features
Glimpse 0.1.0 is based on [GNU Image Manipulation Program 2.10.12](https://www.gimp.org/news/2019/06/12/gimp-2-10-12-released/). It also uses the following dependency package versions:

* [BABL](http://www.gegl.org/babl/) 0.1.68
* [GEGL](http://www.gegl.org/) 0.4.16
* [MyPaint](http://mypaint.org/) 1.3.0

### Graphical User Interface:
* Translation files, code & build files updated so "Glimpse" is displayed
throughout the UI, executables and packages
* Changed the default UI behaviour for a cleaner/more professional look
* Replaced application logo and window/taskbar icons
* Replaced "wilber eek" logo with a new application logo
* Replaced initial splash screen
* Updated upstream icon themes to include our own iconography
* Replaced some links in the "Help" menu
* Removed links to upstream help pages and documentation
* Updated the About window
* Removed code for upstream "easter eggs"
* Refactored version strings and compatibility notices in file save dialog
* Refactored display text for plug-ins, extensions and procedures
* Modified preferences panel to re-brand "Debugging" section and removed
toolbar header checkbox

### Code Improvements:
* Refactored the automated "authors" system for the Glimpse project
* Refactored the build system for the Glimpse project
* Removed some scripts and tooling we do not use with this fork
* Updated the Flatpak build process and removed webkit build step for dev builds
* Provided support for Snapcrafters to package the code through their third
party distribution channel
* Added Travis CI support to sanity check and test builds in version control
* Created a new 32-bit Windows installer with the WiX toolset

### Developer Assistance:
* Added BABL, GEGl and MyPaint dependencies as git submodules pre-set at the
current tagged releases
* Added [Vagrant](https://www.vagrantup.com/) support so the code can be built
& run without needing to install the prerequisites on the host system
* Provided comprehensive build documentation for Windows and Linux in the `HACKING` file and at
https://wiki.glimpse-editor.org/index.php?title=Building_Glimpse
* Improved integration with the GNOME Builder IDE
* Provided new code level documentation of our own (such as code of conduct,
contributing guide, changelog, etc)

### Quality of Life Improvements:
* Removed legacy upstream documentation not needed for this fork
* Changed installation & configuration files location to avoid conflicts
* Changed cached and temporary files location to avoid conflicts
* Changed process identifiers so they do not conflict with other running
instances of the GNU Image Manipulation Program
* Added our own metadata for built and packaged executables
* Removed "Color" icons (duplicates "Legacy")
* Removed "Gray" UI theme (duplicates "System")
* Provided our own AppStream metadata
* Maintained compatibility with existing GNU I.M.P v2.x plug-ins
* Refactored "Created with GIMP" notice to "Created with Glimpse" in the
default save file metadata
* Replaced Windows save file metadata icon
* Re-branded categories used in Plug-in and Procedure browsers

## Credits
We would like to thank everyone who contributed towards making Glimpse 0.1.0 a success, particularly those unnamed individuals who spread the word about our project on social media, shared their feature requests with us and provided feedback to the development team during the beta testing phase.

### Creator
* Bobby Moss

### Maintainers
* Christopher Davis
* Clipsey

### Code Contributors
* Heather Ellsworth
* igalic
* Mathieu Bridon
* psymole

### Documentation Contributors
* chaomodus
* melody

### Artwork Contributors
* James Daniel

### $20+ Tier Sponsor Contributors
* Dominic Watson
* Kretz
* Loren Dias
* Massimo D'Ambrogio
* Roberts-Loux Foundation
* Sami Mannila

### $5+ Tier Backers and One-off Donors
We would like to say a special thank you to all of our financial backers on [Open Collective](https://opencollective.com/glimpse) and Patreon regardless of whether they are listed below or not. Without your help this release would not have been possible, and your continued support is highly appreciated.

* Aalap Mogre
* Brandon 'Spanky' Mills
* G Cowell
* Gino H
* Joe Mooring
* Kevin Rodriguez
* nitrohorse
* Pagrus
* Phie
* Sam Muirhead
* Samuel Pickard
* Stan Sorochan
* Transmutable
* Violet Leonard
