# Backlog

Features mentioned and not yet brainstormed, in dependency order. A line here is a name, a
purpose and what it depends on, plus anything the developer has already said about it, kept in
their words so nothing is lost before its brainstorm. Nothing on this list is designed or
built until it has been through `feature-brainstorm` and has a brief of its own.

## Kit

- **Door wire protocol**: a door describes each screen once, by meaning: menus, text panels,
  prompts, lists, forms, and images with an ANSI fallback. Input comes back as events, such as
  an item chosen or a form submitted, so a hotkey in a terminal and a click on the web mean
  the same. A door can override per front end, with hand-drawn ANSI for terminals and its own
  images or styling for the web; automatic rendering is the default. Depends on: nothing.
- **Host-side renderer**: the kit renders a door's screens as ANSI, honouring the caller's
  negotiated colour tier and graphics, or as HTML. A host such as HeliosDoors uses it, so
  doors improve without being rebuilt. Depends on: door wire protocol.
- **Language SDKs**: SDKs for porting old games to the kit: C and Pascal first, and a few
  other languages later, each with an API shaped like the classic door kits (OpenDoors for C,
  the Pascal door libraries) so a port swaps a library rather than rewriting its input and
  output. Depends on: door wire protocol.
