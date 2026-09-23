# HeliosDoorKit

Wire protocol and multi-language SDK for BBS doors.

Describe a screen once; the kit renders it for whichever front end the caller arrived on. It is not tied to any single BBS: the host side is implemented by HeliosDoors, the door hosting service, and by any other host that speaks the protocol.

## Status: pre-release, built in the open

No version has been released and no tag exists. `main` holds releases only; work lands on
`development` through pull requests, and the issues and the estate's project board show what
is being worked on now.

The project is designed feature-first: the developer writes a brief for each feature in
`features/`, and the specifications in `docs/spec/` are derived from those briefs, with every
section naming the features it serves. `CONSTITUTION.md` holds what is specific to this
project; the principles shared across the estate live in the
[HeliosSkills](https://github.com/HeliosBBS/HeliosSkills) plugin.

## The estate

Part of [Helios](https://github.com/HeliosBBS): the [engine](https://github.com/HeliosBBS/HeliosAdvance),
the [Door Kit](https://github.com/HeliosBBS/HeliosDoorKit), the
[door hosting service](https://github.com/HeliosBBS/HeliosDoors), the
[Portal](https://github.com/HeliosBBS/HeliosPortal) and the
[SIP gateway](https://github.com/HeliosBBS/HeliosSIP). Each project's interface to the engine
is a protocol, a wire format, or nothing at all. This one owns the door wire protocol and consumes nothing from the engine.

## Licence

**Apache License 2.0.** Permissive on purpose: a door built with the kit may be closed-source and commercial, and other BBS software may implement the protocol; nothing in this licence reaches into either.

