# Google sheet Formula UDL (User Defined Language) for Notepad++ 
*gsheet formula sintax highlighting (support English & Italian Formulas)*

Use Notepad++ for google sheet formulas editing and create complex formulas!

Special Colors for all formulas, operators, comments...

# Usage:

Example (Please note, if you’re based in US or Europe, the syntax is a little different (";" instead of ",")

```
=IFERROR(
	IF(PTB!D82+ N("recupera temp max acqua. Però capita che sia invertita con pot. frigo")>1000 ;
		TEXT(CEILING(PTB!E84-L145;1);"#.#");
		TEXT(CEILING(PTB!F82-L145;1);"#.#"))&T(N("di solito F82 è il delta T"));
	"TBD")

	&T(N("
	COMMENTS:
	L145 è num casuale per refresh.
	TBD segnala errore

	"))

```

Inside Notepad++ :
</br>
<img src="https://github.com/adegard/gsheet_notepad-plus-plus/blob/main/Cattura3.JPG"  align="center">

</br>
Then, just copy it inside gsheet Formula field.


# Installation

-Download <a href="https://raw.githubusercontent.com/adegard/gsheet_notepad-plus-plus/main/formula_gsheet_notepad.xml" rel="nofollow">formula_gsheet_notepad.xml</a> (right click Save as...)</br>

*Test method:*</br>
-Go to Language/User define langage/Define language..., import it.</br>

*Official UDL installation*:</br>
-Import the file by placing the file in your userDefineLangs folder and restarting Notepad++. (It is also possible to use the User Defined Language dialog box to Import your file, but that places the UDL in the combined file, which is more complicated to maintain). More details of what those steps entail can be found in the "Import a UDL" section of the official documentation (https://npp-user-manual.org/docs/user-defined-language-system/#import-a-udl).</br>

Please report me any issue.

# Special tips for commenting in formula:

when result is a number, use:
```
+N("my comment")
```
when result is a text, use:
```
&T(N("my comment"))
```
Multi-line commenting:
```
+N("
****
this
is 
multi line
comment
***
")
```

# Notepad++ Forum Thread 
https://community.notepad-plus-plus.org/topic/20237/gsheet-formula-sintax-highlighting/
