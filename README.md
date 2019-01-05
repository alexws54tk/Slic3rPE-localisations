# Localizations for the Slic3r Prusa Edition
https://github.com/prusa3d/Slic3r/tree/master/resources/localization

## Current list

| - | Lang  |  Lines translated | Lines in `.pot` | %% | Last update |
| - | ----- | ---- | ---- | ------ | ------ |
| - | [cs_CZ](localization/cs_CZ/Slic3rPE_cs.po) 	|  989 | 1107 | 89.34% | |
| - | [de_DE](localization/de_DE/Slic3rPE_de.po) 	|  990 | 1107 | 89.43% | |
| - | [en_US](localization/en_US/Slic3rPE_en.po) 	|  770 | 1107 | 69.56% | |
| - | [es](localization/es/Slic3rPE_es.po) 		|  990 | 1107 | 89.34% | |
| - | [fr_FR](localization/fr_FR/Slic3rPE_fr.po) 	|  987 | 1107 | 89.16% | |
| - | [it](localization/it/Slic3rPE_it.po) 		|  990 | 1107 | 89.34% | |
| - | [pl](localization/pl/Slic3rPE_pl.po) 		|  988 | 1107 | 89.25% | |
| + | [ru](localization/ru/Slic3rPE_ru.po) 	| 1153 | 1153 | 100% | 2018-12-16 |
| - | [uk](localization/uk/Slic3rPE_uk.po) 		|  749 | 1107 | 67.66% | |
| - | [zh_CN](localization/zh_CN/Slic3rPE_zh.po) 	|  238 | 1107 | 21.50% | |


# Updating `Slic3rPE.pot` file

```bash
% grep -rn "[\. \(]L([\'\"]" * | cut -d\: -f1 | sort -u | uniq | sort | grep -E "\.[chp][mp]{1,2}$" > resources/localization/list.txt
% xgettext --keyword=L --from-code=UTF-8 --debug -f resources/localization/list.txt -o resources/localization/Slic3rPE.pot
```
