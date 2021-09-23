# Nice backups, dweeb!

A script to check backups made by TWRP 3.5.2\_9-0

This decodes `.ab` files, i.e. backups made through `adb backup --twrp`.

It shows a list of files contained in the backup and warns you if anything is
wrong along the way. It can also make a best effort to recover data from a
broken backup.

## How do I use it?

    ./ab-decode < backup.ab

Don't get that arrow the wrong way around. If you're worried, do this instead:

    cat backup.ab | ./ab-decode

If you want it to try to extract all the files it sees, do this:

    ./ab-decode -e < backup.ab

## This code is pretty nasty

PRs welcome lol

This was written with the goal of figuring out why TWRP was tripping over a
backup I'd just taken hours ago. There was a feeling of urgency to it.

## Why so mean?

The backup software said TWRP to me so I said DWEEB back to its face.
