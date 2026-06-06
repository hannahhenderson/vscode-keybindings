# VS Code keybindings

My personal VS Code `keybindings.json`, kept here so I always have a copy and
can drop it onto a new machine.

The goal: I have years of **IntelliJ muscle memory**, so I rebound the handful
of shortcuts I reach for without thinking. A couple of those collided with VS
Code defaults, so I also had to *unbind* the defaults to make room.

I also **avoid function keys** wherever I can — so where a default sits on an
F-key, I move it onto a ⌘ chord (e.g. references → ⌘R).

**Keys:** ⌘ Cmd · ⇧ Shift · ⌃ Ctrl · ⇥ Tab

## IntelliJ shortcuts I restored

The keys that match what my hands already do in IntelliJ.

| Shortcut | Does |
|---|---|
| ⇥ / ⇧⇥ | Indent / outdent selected lines |
| ⌘[ / ⌘] | Navigate back / forward (history) |

## New VS Code commands

VS Code commands I moved onto different keys — either because their old key got
claimed by the IntelliJ bindings above, or to avoid a function key.

| Shortcut | Command | Why this key |
|---|---|---|
| ⇧⌘B | Toggle sidebar | Moved off ⌘B |
| ⌃⇧⌘B | Run build task | Moved off ⇧⌘B (which became the sidebar) |
| ⌘R | Go to references | Moved off ⇧F12 — avoiding the F-key |

_Freed up along the way and now available: ⌘B, ⌃-, ⌃⇧-._

## Install on a new machine

Copy the file into VS Code's user config directory:

```sh
# macOS
cp keybindings.json ~/Library/Application\ Support/Code/User/keybindings.json
```

(Linux: `~/.config/Code/User/`, Windows: `%APPDATA%\Code\User\`.)

This is a snapshot — if I change my keybindings in VS Code, I re-copy the file
back here and commit.
