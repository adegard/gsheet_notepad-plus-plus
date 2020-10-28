# Google sheet Markup for Notepad++ (support English & Italian Formulas)
Edit Google Sheet Formulas in Notepad++

Use Notepad++ for google sheet formulas editing and create much complex formulas!

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

Also working in Italian...
</br>
<img src="https://github.com/adegard/gsheet_notepad-plus-plus/blob/main/Cattura2.JPG"  align="center">

</br>

# Installation
Download <a href="https://raw.githubusercontent.com/adegard/gsheet_notepad-plus-plus/main/formula_gsheet_notepad.xml" rel="nofollow">formula_gsheet_notepad.xml</a> (right click Save as...)</br>
In Notepad++, go to Language/User define langage/Define language..., import it & enjoy!

# Special tips for commenting in formula:

when result is a number, use:
+N("my comment")

when result is a text, use:
&T(N("my comment"))

Multi-line commenting:

+N("
****
this
is 
multi line
comment
***
")


