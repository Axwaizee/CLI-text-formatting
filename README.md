<h1 align="center">ANSI Escape Codes</h1>

A set of control sequences known as ANSI escape codes can be included into text strings to regulate several aspects of text formatting and display in terminal emulators. These codes are frequently used to add colour, styling, and other effects to the text displayed in the terminal. They are generally supported across several terminals.

#### How ANSI Escape Codes Work:

- **Escape Character (`\x1b` or `\033`):** In most programming languages, the escape character (`\x1b` in JavaScript, Rust, and Go, or `\033` in C, C++, Java and Python) is used to begin an ANSI escape code. The escape code sequence starts with this character.


- **Numeric Codes:** Numerical codes are used to express various formatting options after the escape character. For instance, `\x1b[91m` denotes the bright red foreground colour setting.

- **Reset Code (`\x1b[0m`):** Reset codes are frequently used to undo formatting modifications. For instance, `\x1b[0m` returns text formatting to its initial configuration.


#### Typical Use Cases:

- **Text Colouring:** To alter the colour of text, both foreground and background, ANSI escape codes are commonly utilised.

- **Text Styles:** ANSI escape codes can be used to apply bold, italic, underlining, and other text styles.

- **Special Effects:** Certain codes offer extra effects like framing or blinking text.


#### Note:

- **Cross-Language Compatibility:** Although most programming languages accept ANSI escape codes, there may be minor differences in the syntax for some special codes and escape characters.

- **Terminal Emulator Dependent:** Depending on the terminal emulator being utilised, ANSI escape codes may or may not work. Not every terminal may support every functionality.

<br><br>
<h1 align="center">ANSI Escape Codes for Text Formatting</h1>

| Code | Style/Color | Description |
|------|-------------|-------------|
| 1    | Bold        | Increases text intensity or sets bold text. |
| 2    | Faint       | Decreases text intensity. |
| 3    | Italic      | Italicizes text. |
| 4    | Underline   | Underlines text. |
| 5    | Blink       | Blinks text (not widely supported). |
| 6    | Rapid Blink | Rapidly blinks text (not widely supported). |
| 7    | Inverse     | Inverts background and foreground colors. |
| 8    | Conceal     | Hides text (not widely supported). |
| 9    | Crossed Out | Crosses out text (not widely supported). |
| 10-19| Default Font | Set default text style (not widely supported). |
| 20   | Fraktur     | Fraktur style (rarely supported). |
| 21   | Bold Off    | Turn off bold (not widely supported). |
| 22   | Normal Intensity | Reset intensity (not widely supported). |
| 23   | Italic Off  | Turn off italic (not widely supported). |
| 24   | Underline Off | Turn off underline (not widely supported). |
| 25   | Blink Off   | Turn off blink (not widely supported). |
| 27   | Inverse Off | Turn off inverse (not widely supported). |
| 28   | Reveal      | Reveal hidden text (not widely supported). |
| 29   | Not Crossed Out | Not crossed-out text (not widely supported). |

### Foreground Colors:
| Code | Color       | Description |
|------|-------------|-------------|
| 30-37| Dark Foreground Colors | Various dark colors. |
| 38   | Extended Foreground | Specify RGB foreground color (not widely supported). |
| 39   | Default Foreground | Default foreground color. |

### Background Colors:
| Code | Color       | Description |
|------|-------------|-------------|
| 40-47| Dark Background Colors | Various dark background colors. |
| 48   | Extended Background | Specify RGB background color (not widely supported). |
| 49   | Default Background | Default background color. |

### Bright Foreground Colors:
| Code | Color       | Description |
|------|-------------|-------------|
| 90-97| Bright Foreground Colors | Various bright colors. |

### Bright Background Colors:
| Code | Color       | Description |
|------|-------------|-------------|
| 100-107| Bright Background Colors | Various bright background colors. |

### Miscellaneous:
| Code | Style/Effect | Description |
|------|--------------|-------------|
| 50   | Reset Font   | Reset font to default (not widely supported). |
| 51   | Framed       | Frame text (not widely supported). |
| 52   | Encircled    | Encircle text (not widely supported). |
| 53   | Overlined    | Draw line above text (not widely supported). |
| 54   | Not Overlined| Cancel overlined effect (not widely supported). |
| 55-89| Reserved     | Reserved for future standardization (not widely supported). |
| 98   | Default Foreground RGB | Reset foreground color to default (not widely supported). |
| 99   | Default Background RGB | Reset background color to default (not widely supported). |

### Hide and Unhide Cursor

You can hide the cursor by using `[?25l` and unhide back using `[?25h`. For instance, `\x1b[?25l` in JavaScript, Rust, and Go or `\033[?25l` in C, C++, Java and Python