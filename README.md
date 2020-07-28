# Defenders of Skyrim - i18n
Repository for all localizations

## How to contribute
0. Make fork of this repository to your account
1. Clone repository to computer
2. Choose which mod you want to translate
3. Translate mod
4. Make pull request from your repository
5. PROFIT?

## Repository structure
For translation i'm using ESP/ESM Translator. It can save and load translations from xml files, so it can be edited in *notepad*

In repository folder you can see, that each mod comes in own folder:
| Folder name | Mod name | File name |
| ------ | ------ | ------ |
| Main | Defenders of Skyrim | Defenders_of_Skyrim_EN-*lang*.xml |
| Armory | Defenders of Skyrim - Armory | Defenders_of_Skyrim_Armory_EN-*lang*.xml |
| Artifacts | Defenders of Skyrim - Artifacts | Defenders_of_Skyrim_Artifacts_EN-*lang*.xml |
| Wardrobe | Defenders of Skyrim - Wardrobe | Defenders_of_Skyrim_Wardrobe_EN-*lang*.xml |

In *Main* folder also you can find files, which have suffix **Followers**, etc. - it's also goes to main mod, just now for more bug-free development it's separated.

*lang* - destination language (RU, DE, etc.)

### Translation
To add new language, just copy and paste in same folder existed file (which ends with EN-RU suffix) and change destination language to one of supported by Skyrim:
* English - EN
* Russian - RU
* French - FR
* Italian - IT
* German - DE
* Spanish - ES
* Polish - PL
* Traditional Chinese - CN
* Japanese - JP

This list are taken from https://help.bethesda.net/app/answers/detail/a_id/31431/~/how-do-i-change-the-language-in-skyrim-on-pc%3F and it's to Skyrim SE, but i assume that in Legendary Edition same languages available.

You can reference to translations in DOTA2, DOTA Underlords and other games to translate item names, descriptions or character names. Also you can visit GitHub wiki to view [glossary](https://github.com/Defenders-of-Skyrim/i18n/wiki).

### XML Structure
Each file contains some XML tags, which represents some text:
```html
<ESP>
    <GRUP>MGEF</GRUP>
    <ID>010022FF</ID>
    <EDID>DoS_Artifacts_Desolator1Effect</EDID>
    <CHAMP>FULL</CHAMP>
    <ORIGINAL>Corruption</ORIGINAL>
    <TRADUIT>Порча</TRADUIT>
    <INDEX>1</INDEX>
    <STATUS>98</STATUS>
    <IDSTEXTE>25</IDSTEXTE>
    <COMMENTAIRE />
    <ICON>-1</ICON>
</ESP>
```
You need **TRADUIT** tag - it contains translated strings. When you translate string template, instead of <> use escaped characters as \&lt; or \&gt;, ex.
```html
<ORIGINAL>Your attacks reduce the target's armor by &lt;mag&gt; for &lt;dur&gt; seconds.</ORIGINAL>
```

# What after?
You would be a good Dovakhin, which helps translating mods to other languages.