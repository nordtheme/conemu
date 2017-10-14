<p align="center"><img src="https://cdn.rawgit.com/arcticicestudio/nord-conemu/develop/assets/nord-conemu-banner.svg"/></p>

<p align="center"><img src="https://assets-cdn.github.com/favicon.ico" width=24 height=24/> <a href="https://github.com/arcticicestudio/nord-conemu/releases/latest"><img src="https://img.shields.io/github/release/arcticicestudio/nord-conemu.svg?style=flat-square"/></a> <a href="https://github.com/arcticicestudio/nord/releases/tag/v0.2.0"><img src="https://img.shields.io/badge/Nord-v0.2.0-88C0D0.svg?style=flat-square"/></a></p>

<p align="center"><a href="https://github.com/arcticicestudio/nord-conemu/blob/v0.1.0/CHANGELOG.md"><img src="https://img.shields.io/badge/Changelog----81A1C1.svg?style=flat-square"/></a></p>

<p align="center">An arctic, north-bluish clean and elegant <a href="https://conemu.github.io">ConEmu</a> color scheme.</p>

<p align="center">Designed for a fluent and clear workflow.<br>
Based on the <a href="https://github.com/arcticicestudio/nord">Nord</a> color palette.</p>

---

<p align="center"><img src="https://raw.githubusercontent.com/arcticicestudio/nord-conemu/develop/assets/scrot-hero.png"/></p>

## Getting started

### Installation

If you never added or created a custom color scheme, your `ConEmu.xml` will not contain the necessary `Colors` key. You can generate it by opening the *Settings* and navigate to *Features* > *Colors* in the tree view. Create a new custom color theme with any name and press on the <kbd>Save</kbd> button. This will automatically generate the `Colors` key in your `ConEmu.xml` configuration file.

Open your `ConEmu.xml` configuration file to add the Nord ConEmu theme key. Please read the official documentation chapter about the [ConEmu settings storage][conemu-doc-settings-storage] to get the file path based on your setup.

Paste the content of the [`nord-conemu.xml`][nord-conemu-xml] color scheme file (the comment header is optional and can be left out) at the end of the `Colors` key which should start like the following:

```xml
<key name="Colors" modified="2017-10-14 09:05:45" build="170910">
  <value name="Count" type="dword" data="00000001"/>
  <key name="Palette1" modified="2017-10-14 09:05:45" build="170910">
```

Update the palette number (`<key name="PaletteX"`) accordingly. For example, if you have one custom color palette already, the Nord ConEmu theme should be `Palette2`:

```xml
<key name="Palette2" modified="2017-10-14 09:05:45" build="170910">
  <value name="Name" type="string" data="Nord"/>
```

Make sure to increase the value for `Count` key right after the `Colors` key as well. It should equal to the total number of palettes:

```xml
<value name="Count" type="dword" data="00000002"/>
```

This example shows the complete `Colors` key when only the Nord ConEmu color scheme has been installed:

```xml
<key name="Colors" modified="2017-10-14 09:05:45" build="170910">
  <value name="Count" type="dword" data="00000001"/>
  <key name="Palette1" modified="2017-10-14 09:05:45" build="170910">
    <value name="Name" type="string" data="Nord"/>
    <value name="ExtendColors" type="hex" data="00"/>
    <value name="ExtendColorIdx" type="hex" data="0e"/>
    <value name="TextColorIdx" type="hex" data="10"/>
    <value name="BackColorIdx" type="hex" data="10"/>
    <value name="PopTextColorIdx" type="hex" data="10"/>
    <value name="PopBackColorIdx" type="hex" data="10"/>
    <value name="ColorTable00" type="dword" data="0040342e"/>
    <value name="ColorTable01" type="dword" data="00926c47"/>
    <value name="ColorTable02" type="dword" data="00518e6c"/>
    <value name="ColorTable03" type="dword" data="008c8d54"/>
    <value name="ColorTable04" type="dword" data="006a61bf"/>
    <value name="ColorTable05" type="dword" data="00ad8eb4"/>
    <value name="ColorTable06" type="dword" data="008bcbeb"/>
    <value name="ColorTable07" type="dword" data="00e9ded8"/>
    <value name="ColorTable08" type="dword" data="006a564c"/>
    <value name="ColorTable09" type="dword" data="00c1a181"/>
    <value name="ColorTable10" type="dword" data="008cbea3"/>
    <value name="ColorTable11" type="dword" data="00bbbc8f"/>
    <value name="ColorTable12" type="dword" data="003c3483"/>
    <value name="ColorTable13" type="dword" data="007b5683"/>
    <value name="ColorTable14" type="dword" data="0031a4db"/>
    <value name="ColorTable15" type="dword" data="00f4efec"/>
    <value name="ColorTable16" type="dword" data="00000000"/>
    <value name="ColorTable17" type="dword" data="00800000"/>
    <value name="ColorTable18" type="dword" data="00008000"/>
    <value name="ColorTable19" type="dword" data="00808000"/>
    <value name="ColorTable20" type="dword" data="00000080"/>
    <value name="ColorTable21" type="dword" data="00800080"/>
    <value name="ColorTable22" type="dword" data="00008080"/>
    <value name="ColorTable23" type="dword" data="00c0c0c0"/>
    <value name="ColorTable24" type="dword" data="00808080"/>
    <value name="ColorTable25" type="dword" data="00ff0000"/>
    <value name="ColorTable26" type="dword" data="0000ff00"/>
    <value name="ColorTable27" type="dword" data="00ffff00"/>
    <value name="ColorTable28" type="dword" data="000000ff"/>
    <value name="ColorTable29" type="dword" data="00ff00ff"/>
    <value name="ColorTable30" type="dword" data="0000ffff"/>
    <value name="ColorTable31" type="dword" data="00ffffff"/>
  </key>
</key>
```

### Activation

Open your *Settings* and navigate to *Features* > *Colors* in the tree view. Select `Nord` from the *Scheme* drop-down menu and save by pressing on the <kbd>Save settings</kbd> button.
  
### Contribution

Please report issues/bugs, feature requests and suggestions for improvements to the [issue tracker](https://github.com/arcticicestudio/nord-conemu/issues).

<p align="center"><img src="https://cdn.rawgit.com/arcticicestudio/nord/develop/src/assets/banner-footer-mountains.svg" /></p>

<p align="center">Copyright &copy; 2017 Arctic Ice Studio</p>

<p align="center"><a href="http://www.apache.org/licenses/LICENSE-2.0"><img src="https://img.shields.io/badge/License-Apache_2.0-5E81AC.svg?style=flat-square"/></a> <a href="https://creativecommons.org/licenses/by-sa/4.0"><img src="https://img.shields.io/badge/License-CC_BY--SA_4.0-5E81AC.svg?style=flat-square"/></a></p>

[conemu-doc-settings-storage]: https://conemu.github.io/en/ConEmuXml.html
[nord-conemu-xml]: https://github.com/arcticicestudio/nord-conemu/blob/develop/src/nord-conemu.xml
