# Highly Featured LaTeX Novel Template

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![LuaLaTeX](https://img.shields.io/badge/Engine-LuaLaTeX-blue)](https://www.luatex.org/)

Professional LaTeX template for typographical featured novels. Designed for authors who want to incorporate typographical experimentation into their narrative structure.

![First Sample Page](images/novel_template_page-0003.jpg)
![Second Sample Page](images/novel_template_page-0004.jpg)

## Features

- **Glitch Text Effects**: Three unreadable font styles for memory distortion sequences
- **Multiple Chapter Styles**: 4 distinctive chapter heading designs
- **Sensory Descriptions**: Context-aware formatting for sight/sound/touch/smell/taste
- **Battle Scene Formatting**: Dual-column action sequences with power level indicators
- **Character Entries**: 3 style variations (classical/modern/minimal)
- **System Status Blocks**: Tech-inspired diagnostic readouts
- **Advanced Scene Separation**: 5 thematic break styles with ornaments
- **Margin Notes & Annotations**: For editorial comments and translations
- **Danger Indicators**: Custom stamps and progress bars for threat levels
- **Flexible Metadata**: Support for epigraphs, letters, and flashbacks

## Installation

1. **Required Fonts** (included in `/fonts`):

   ```bash
   # Linux/macOS
   cp fonts/* ~/.fonts/
   # Windows: Copy to C:\Windows\Fonts
   ```

2. **Compilation**:

   ```bash
   lualatex novel_template.tex
   ```

## Usage

### Basic Structure

```latex
\documentclass[11pt, openany]{book}
\usepackage{novel-template}

\begin{document}
\chapter{Echoes of Yesterday}
\dropcap[3]{M}y glitched memory...
\end{document}
```

### Key Elements

**Chapter Definition**:

```latex
\setchapterstyle{2} % Change chapter style (1-4)
\chapter{Fractured Realities}
```

**Dialogue & Thoughts**:

```latex
\dialogue{Where am I?} \charname{Eliza} asked.
\thought{This doesn't feel real...}
```

**Scene Separation**:

```latex
\scenesep[3] % Decorative symbols
\minorscenebreakline % Thin horizontal rule
```

## Customization

### Chapter Styles

```latex
\setchapterstyle{3} % 1=Classic, 2=Modern, 3=Minimalist, 4=Vintage
```

### Font Families

```latex
\newfontfamily\myfont{New Font Name}
\renewcommand{\titlefont}{\myfont}
```

### Color Scheme

```latex
\definecolor{mygray}{RGB}{64,64,64}
\renewcommand{\memoryglitch}[2][]{\color{mygray}...}
```

## Examples

**Chapter Opening**:

```latex
\dropcap[3]{T}he machine \sfx{hummed}...
\sensory[strong]{sound}{Deafening silence}
```

**Battle Sequence**:

```latex
\battleline{\charname{Eliza} parried}{The creature \emph{roared}}
\powerlevel[Red]{0.85} % 85% red power bar
```

**System Readout**:

```latex
\begin{systemstatus}
  MEMORY_INTEGRITY: 43%
  CORRUPTION_LEVEL: SEVERE
\end{systemstatus}
```

## Contributing

Contributions welcome! Please:

1. Open an issue to discuss changes
2. Fork the repository
3. Commit changes
4. Push to branch
5. Open Pull Request

## License

MIT License - See [LICENSE](LICENSE) file

## Full Example

![images/novel_template_page-0001](images/novel_template_page-0001.jpg)
![images/novel_template_page-0002](images/novel_template_page-0002.jpg)
![images/novel_template_page-0003](images/novel_template_page-0003.jpg)
![images/novel_template_page-0004](images/novel_template_page-0004.jpg)
![images/novel_template_page-0005](images/novel_template_page-0005.jpg)
![images/novel_template_page-0006](images/novel_template_page-0006.jpg)
![images/novel_template_page-0007](images/novel_template_page-0007.jpg)
![images/novel_template_page-0008](images/novel_template_page-0008.jpg)
![images/novel_template_page-0009](images/novel_template_page-0009.jpg)
![images/novel_template_page-0010](images/novel_template_page-0010.jpg)
