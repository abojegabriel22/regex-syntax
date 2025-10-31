Regular Expressions are patterns used to match, search, and manipulate text.
syntax:

.     ---------------  Any single character except newline
^     ---------------- start of string
$     ----------------  End of string
*     -------------     0 or more times
+     ---------------   1 or more times
?     -----------       0 or 1 time (optional)
[]     -------------    character set         example /gr[ae]y/  => gray, grey, you
[^]   -----------       negated set    => not any character inside the set    => .match(/[^0-9]/) "1324", "TEN" "twenty" "15" "490" "@" "$" "!" "*" a-zA-Z !@#$%^&*()_
{n}   ----------------- exactly n times  => {} => a{3} meanining aaa 4{2} 44, 
{n,}  ----------------  n or more times   => a{2,} 2 or more a's example: aa, aaa, aaaa, aaaaa, aaaaa
{n,m}  ---------------- between n and m times  => a{2,5}  => aa aaa aaaa aaaaa aaaaaa   // abojegabriel20@gmail.co
()    ---------------   group parenthesis  => group things together => (ha)+  => matches ha, hahaha, hahahahaha, hahahaha hia => use it to capure parts of a match => "I love cats".match(/cats/) // ["cats"]
`     --------------    ` a literal dot means any character
\     ---------------   escape special character

| the Pipe  ------- Or (either this or that) => cats|dogs 

shortcuts

\d    --------------    digit    (0-9)         examples /\d\d/ matchs 12, 45
\D    -------------     non-digit (\D)        A, B, Z !,@
\w    --------------    word character (a-z, A-Z, 0-9, _)   /\w+/        Aboje_123
\W    --------------    non-word character  => /\W/  @!$%^&
\s    --------------    whitespace   => "     "  /\s/
\S    --------------    non-whitespace => /\S/  =>  "a", "aboje" => oche_james
\b    --------------    word boundary (edge of a word)  => /\bcat\b/  => "cat" but not "catalog"
\B    --------------    non-word boundary  => /\Bcat/ "catalog","educate","communication","COMMUNICATION"



flags (Modifiers)

g     ---------------    global (find all matches)

i     ---------------    case-insensitive Abojegabriel, abojegabriel

m     ---------------    Multiline




examples each:
using .    -----------   /c.t/                ---- "cat", "cot", "cut"
it matches any single character except new line

^          -----------   /^Hi/               -----"Hi there"

$    -----------       /end$/            ---------- "the end"

*    r

examples

const text = "I have 12 cats and 3 dogs."
console.log(text)
console.info()


console.log()  // you use console.log() javascript inbuilt function to print 3 things  // but normally 2 things
these two things are:

your success message => console.log(),

console.info() => display information

console.log()

error message
console.log(), console.error()

console.warn(text)
with regex now
console.log(text.match(/\d/g))

in javascript
"sting"
{

}
["tin", "meat", "gas"]  = array of items in javascript

console.log(text.match(/\d/g))
VM453:1 (3) ['1', '2', '3']

console.log(text.match(/[a-z]+/gi))

console.log(text.match(/[a-z]+/gi))
VM457:1 (5) ['I', 'have', 'cats', 'and', 'dogs']

console.log(text.match(/[a-zA-Z0-9]+/g))

console.log(text.match(/[a-zA-Z0-9]+/g))
VM465:1 (7) ['I', 'have', '12', 'cats', 'and', '3', 'dogs']
undefined
console.log(text.match(/[a-z0-9]+/g))
VM471:1 (6) ['have', '12', 'cats', 'and', '3', 'dogs']
undefined
console.log(text.match(/[a-zA-Z]+/g))
VM477:1 (5) ['I', 'have', 'cats', 'and', 'dogs']


real world implementation with email
=> find all emails:
/[\w.-]+@[\w.-]+/        => user@gmail.com user123@gmail.com user @gmail.com


find all numbers
/\d+/g                   => 2024, 300 etc

check if link starts with "https"
/^https/                => must starts with https://

replace space with "_"
/g, "_"                 => "hello world" => "hello_world"

check if strings ends with .jpg
/\.jpg$/i                         => photo.jpg, Photo.JPG, photo.png


what man understands
degrees (celcius)

what computer understands 
radians


2π radians
Also, since an angle in radians is defined as the ratio of two lengths, L/r, it is dimensionless. Since 90° = π / 2 radians, then four significant figures, one radian equals 180° / π = 57.30°. There are 2π radians in a full circle. (So ​​2π radians should equal 360°.

sin(30)
sin(30 + 15)
sin(30 + 12 + 15)


replace(/sin\(([^)]+)\)/g, 'Math.sin(($1)*Math.PI/180)')

.replace()
//g,
sin\(([^)]+\))  
Math.sin(($1)*Math.PI/180)

once you write sin(30)

Math.sin(($1)*Math.PI/180)


// there are
Math.sin()
Math.cos()
Math.tan()

Math.asin()
Math.acos()
Math.atan()

sin(30)

