# refind-elementary-test

1. Download rEFInd (http://www.rodsbooks.com/refind/getting.html) as a "Binary zip file" and decompress it. 
2. Copy the `refind` Directory that is inside to `/boot/efi/EFI/refind/`.
3. Copy the `refind.conf` from this repository to that same directory.
4. Enable it with `efibootmgr` or through your Computers Setup Utility.
5. Install elementary OS without Grub by Booting to the live Session and using `ubiquity -b`
6. Finish installing and restart.

Elementary should now start through refind, if not this guide is incomplete.

It should still show ugly boot messages though, for that we have 2 more things to do:

1. Copy the `refind_linux.conf` to your Installations `/boot/` directory, this will make everything load nice and graphically.
2. Copy the `.VolumeIcon.png` in this repository to your filesystem root: `/`
