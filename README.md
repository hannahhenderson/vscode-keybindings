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

| Shortcut | Does | IntelliJ habit |
|---|---|---|
| ⇥ / ⇧⇥ | Indent / outdent selected lines | IntelliJ indents the selection with Tab |
| ⌘[ / ⌘] | Navigate back / forward (history) | IntelliJ's back/forward jumps |
| ⌘R | Go to references | Replaces the ⇧F12 default — avoiding the F-key |
| ⇧⌘B | Toggle sidebar | — |
| ⌃⇧⌘B | Run build task | Moved here to free up ⇧⌘B |

## VS Code defaults I overwrote

These are the `-command` entries in the file — they remove a default so the
binding above can take over.

| Shortcut | Was (VS Code default) | Freed for |
|---|---|---|
| ⌘[ | Outdent lines | Navigate back |
| ⌘] | Indent lines | Navigate forward |
| ⌘B | Toggle sidebar | (freed) |
| ⇧⌘B | Run build task | Toggle sidebar |
| ⌃- | Navigate back | (freed) |
| ⌃⇧- | Navigate forward | (freed) |

## Install on a new machine

Copy the file into VS Code's user config directory:

```sh
# macOS
cp keybindings.json ~/Library/Application\ Support/Code/User/keybindings.json
```

(Linux: `~/.config/Code/User/`, Windows: `%APPDATA%\Code\User\`.)

This is a snapshot — if I change my keybindings in VS Code, I re-copy the file
back here and commit.
