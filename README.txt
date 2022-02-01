# Above and Beyond Typus

**File names**

For countries:
TAG - NAME.txt
TAG may contain letters and digits, but must not start with a digit.
NAME may contain letters and spaces.

For provinces:
ID - NAME.txt
ID may contain digits only (duh).
NAME may contain letters, digits and spaces.


**Encoding**

Localisation (`.yml`) files -- obligatorily UTF-8-BOM.
Don't use characters not supported by CP-1252.

Everything else -- CP-1252 (Windows West European)


**End of line**

Use Windows format CR LF only (regexp: \r\n).


**White spaces**

For convenience, in Notepad++ go to:
View / Show Symbol
and choose:
Show White Space and TAB

and go to:
Settings / Preferences / Language
and choose:
Tab size: 3

Never use spaces for positioning or indentation.
Never use more than one space in a row.


**Indentation**

Always use tabs.
Don't indent the first level nodes.
For the other ones, always use one tab more than their parent node:

ex.
abc = {
	def = {
		ghi = {
			XXX
		}
	}
}


**Comments**

Don't use following _singular_ characters in comments:
{ } [ ] ( ) < >

`# ???` -- uncertain.
`# XXX` -- go back to it.
`# BT` -- a node added by BT.
`# BT; comment` -- a node added by BT with a comment.
`# BT; N` -- a node's value changed by BT; N = its vanilla value (number or string).
`# BT had N` -- BT N value (number or string) replaced.

Add your name to your comments.


**Internal names**

For areas\regions:
NAME_area
NAME_region
NAME must not contain spaces; may contain letters, underscores and digits, but must not start with a digit.


**Files removed from BT 13.0.13**

`common\bookmarks`

all not supported ones -- see: `.mod\0BT.131.mod`


`common\cultures`
`
01_bt_defunct_cultures.txt` -- see: `00_cultures.txt`


`common\event_modifiers`
`
01_mission_modifiers.txt` -- identical to 1.30.4


`common\scripted_triggers`
`
00_scripted_triggers.txt` -- identical to 1.30.4
(restored per 1.31.5.2)


`common\units`

40 units identical to vanilla
1 unused file


`gfx\flags`

3 flags identical to vanilla


`history\provinces`

156 unused province files


`events`
`
Catholic.txt` -- doesn't need adjustment for add_reform_desire`
Dynastic.txt` -- doesn't need adjustment for add_reform_desire`
flavorCYP.txt` -- identical to 1.31.5.2`
ThePapacy.txt` -- identical to 1.31.5.2
