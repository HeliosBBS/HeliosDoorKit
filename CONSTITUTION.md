# Constitution

The estate's shared constitution, in the `helios` plugin, is loaded first in every session and
holds the principles: authority from features down, security designed in, multi-node from the
start, the estate and its contracts, the spec rules. This file adds only what is specific to
HeliosDoorKit, and is loaded right after it, unchanged.

## Role

Describe a screen once; the kit renders it for whichever front end the caller arrived on. It is not tied to any single BBS: the host side is implemented by HeliosDoors, the door hosting service, and by any other host that speaks the protocol.

It owns the door wire protocol and consumes nothing from the engine. An interface it owns changes here first, with a version,
before any consumer moves; an interface it consumes is cited by name and version from the
contracts register, never restated.

## How this file is used

Loaded after the shared constitution by every skill, every prompt and every loop iteration. A
change to it is a pull request the developer approves, and nothing else edits it.
