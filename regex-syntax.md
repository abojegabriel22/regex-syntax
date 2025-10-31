Regular Expressions are patterns used to match, search, and manipulate text.
syntax:

.     ---------------  Any single character except newline
^     ---------------- start of string
$     ----------------  End of string
*     -------------     0 or more times
+     ---------------   1 or more times
?     -----------       0 or 1 time (optional)
[]     -------------    character set
[^]   -----------       negated set
{n}   ----------------- exactly n times
{n,}  ----------------  n or more times
{n,m}  ---------------- between n and m times
()    ---------------   group
`     --------------    `
\     ---------------   escape special character

shortcuts

\d    --------------    digit
\D    -------------     non-digit
\w    --------------    word character (a-z, A-Z, 0-9, _)
\W    --------------    non-word character
\s    --------------    whitespace
\S    --------------    non-whitespace
\b    --------------    word boundary
\B    --------------    non-word boundary



flags (Modifiers)

g     ---------------    global (find all matches)

i     ---------------    case-insensitive

m     ---------------    Multiline