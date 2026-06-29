# labelle-sdl-gamepad

Shared windowless-SDL desktop gamepad source for
[labelle](https://github.com/labelle-toolkit) backends (core#28) — reads
controllers GLFW can't decode (Switch-mode / 8BitDo via HIDAPI). Extracted from
the assembler's in-tree `backends/sdl_gamepad/` so out-of-tree backends (e.g.
`labelle-bgfx`) can depend on it as a versioned package instead of a vendored
copy (labelle-assembler#386). Depends on `labelle-core` for the frozen
GamepadEvent/GamepadDescription contract.
