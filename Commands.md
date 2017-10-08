Command|Elements Popped|Description|
-------|---------------|-----------|
`ǝ` | pops `a,b,c` | insert b into a on location c
`ʒ` | pops `a` | filter a when the result of code == 1: usage ʒCODE}
`α` | pops `a,b` | push absolute difference of a and b
`β` | pops `a,b` | push a converted from base b (arbitrary)
`γ` | pops `a` | push a split into chunks of consecutive equal elements
`δ` | pops `a,b` | get the next command, push double vectorized command
`ε` | pops `a` | apply each on a: usage εCODE}
`ζ` | pops `a,(b)` | push zipped a with filler b (standardized to space)
`η` | pops `a` | push prefixes(a)
`θ` | pops `a` | push a[-1]
`в` | pops `a,b` | push a converted to base b (arbitrary)
`м` | pops `a,b` | push a.remove(all elements of b)
`н` | pops `a` | push a[0]
`Θ` | pops `a` | push 05AB1E truthified a (a == 1)
`Σ` | pops `a` | sort a by the result of code: usage ΣCODE}
`Ω` | pops `a` | push random_pick(a)
`≠` | pops `a` | push 05AB1E falsified a (a != 1)
`∊` | pops `a` | push vertically mirrored a
`∍` | pops `a,b` | push a extended/shortened to length b
`∞` | pops `a` | push mirrored a
`!` | pops `a,` | push factorial(a)
`#` | pops `a` | if true: break/end (used in infinite loops)
`#` | pops `a` | if contains spaces, split on spaces
`%` | pops `a,b` | push (a % b)
`&` | pops `a,b` | push a AND b
`(` | pops `a` | push -a
`*` | pops `a,b` | push (a * b)
`+` | pops `a,b` | push (a + b)
`,` | pops `a` | print(a)
`-` | pops `a,b` | push (a - b)
`/` | pops `a,b` | push (a / b)
`:` | pops `a,b,c` | a.replace(b, c) / infinite replacement
`;` | pops `a` | push a / 2
`<` | pops `a` | push a - 1
`>` | pops `a` | push a + 1
`?` | pops `a` | print a no newline
`@` | pops `a` | pop and push the element at index a in the stack (leftmost element = index 0)
`B` | pops `a,b` | push base(a, b)
`C` | pops `a` | push int(a, 2)
`D` | pops `a` | push a, a
`F` | pops `a` | for N in range(0, a) { }: F(commands)} / N = variable
`G` | pops `a` | for N in range(1, a) { }: F(commands)} / N = variable
`H` | pops `a` | push int(a, 16)
`J` | pops `a` | push ''.join(a) if a is list / if not, then push ''.join(stack)
`K` | pops `a,b` | push a with no b's
`L` | pops `a` | push [1 .. a]
`O` | pops `a` | push total sum (only on lists)
`P` | pops `a` | push total product (only on lists)
`Q` | pops `a,b` | push a == b (bool)
`R` | pops `a` | push reversed(a)
`S` | pops `a` | push all chars a seperate
`U` | pops `a` | assign X to a
`V` | pops `a` | assign Y to a
`^` | pops `a,b` | push a XOR b
`_` | pops `a` | push negative bool
``` | pops `a` | push all the items of a into the stack
`a` | pops `a` | push is_alpha(a)
`b` | pops `a` | push bin(a)
`c` | pops `a,b` | push a nCr b
`d` | pops `a` | push is_number(a)
`e` | pops `a,b` | push a nPr b
`f` | pops `a` | push list of prime factors (no duplicates)
`g` | pops `a` | push length of a
`h` | pops `a` | push hex(a)
`i` | pops `a` | if statement: iTHEN}: if true { then }
`j` | pops `a` | max_a_spaces.join(stack)
`k` | pops `a,b` | push 0-indexed index of b in a (-1 when not found)
`l` | pops `a` | push lower_case(a)
`m` | pops `a,b` | push a**b
`n` | pops `a` | push a**2
`o` | pops `a` | push 2**a
`p` | pops `a` | push isPrime(a)
`s` | pops `a,b` | push b,a
`t` | pops `a` | push sqrt(a)
`u` | pops `a` | push upper_case(a)
`v` | pops `a` | range loop: for y in a (y = string, N = index)
`x` | pops `a` | push a, a * 2
`z` | pops `a` | push 1 / a
`{` | pops `a` | push sorted a
`~` | pops `a,b` | push a OR b
`Λ` | pops `a,b,c` | store a canvas with {a: num, b: filler, c: pattern} (todo: docs)
`‚` | pops `a,b` | push [a, b]
`ƒ` | pops `a` | push for N in range(0, a + 1)
`†` | pops `a,b` | push a with b filtered to the front
`‡` | pops `a,b,c` | push a.transliterate(b -> c)
`ˆ` | pops `a` | add to global array
`‰` | pops `a,b` | push a divmod b
`Š` | pops `a,b,c` | push c,a,b
`‹` | pops `a,b` | push a < b
`Œ` | pops `a` | push substrings(a)
`Ć` | pops `a` | push enclosed a: a + a[0]
`ƶ` | pops `a` | push lifted a, each element is multiplied by its index (1-indexed)
`Ā` | pops `a` | push truthified a
`–` | pops `a` | if 1, print N (used in loops)
`—` | pops `a` | if 1, print y (used in loops)
`˜` | pops `a` | push deep flattened a
`™` | pops `a` | push title_cased(a)
`š` | pops `a` | push switch_cased(a)
`›` | pops `a,b` | push a > b
`œ` | pops `a` | push permutations(a)
`ć` | pops `a` | push head_extracted a: a[1:], a[0] 
`Ÿ` | pops `a,b` | push [a, ..., b]
`¡` | pops `a,b` | push a.split(b)  
`¢` | pops `a,b` | push a.count(b)
`£` | pops `a,b` | push a[0:b]
`¥` | pops `a` | push delta's a
`¦` | pops `a` | push a[1:]
`§` | pops `a` | push str(a)
`¨` | pops `a` | push a[0:-1]
`ª` | pops `a` | push sentence_cased(a)
`«` | pops `a,b` | push concatenated(a, b)
`°` | pops `a` | push 10 ** a
`±` | pops `a` | push bitwise not a
`µ` | pops `a` | while counter_variable != a, do...
`·` | pops `a` | push 2 * a
`¸` | pops `a` | push [a]
`»` | pops `(a)` | if list, join list by newlines, else join stack by newlines
`½` | pops `a,` | if 1, then counter_variable += 1
`¿` | pops `a` | push gcd(a)
`À` | pops `a` | push a rotated 1 left
`Á` | pops `a` | push a rotated 1 right
`Â` | pops `a` | push bifurcated a
`Ã` | pops `a,b` | push a.keep(b)
`Ä` | pops `a` | push abs(a)
`Æ` | pops `a` | push reduced substraction a
`Ç` | pops `a` | push ASCII value of a
`È` | pops `a` | push a % 2 == 0 (is even)
`É` | pops `a` | push a % 2 == 1 (is uneven)
`Ê` | pops `a,b` | push a != b
`Ë` | pops `a` | push 1 if all equal else 0
`Ì` | pops `a` | push a + 2
`Í` | pops `a` | push a - 2
`Ï` | pops `a,b` | push the elements from a at which the same index at b is 1
`Ñ` | pops `a` | push divisors(a)
`Ò` | pops `a` | push list of prime factors (with duplicates)
`Ó` | pops `a` | push list of exponents of prime factors (2^a, 3^b, 5^c, 7^d, etc.)
`Ô` | pops `a` | push connected uniquified a
`Õ` | pops `a` | push euler_totient(a)
`Ö` | pops `a,b` | push a % b == 0
`×` | pops `a,b` | push a × b (strings)
`Ø` | pops `a` | push ath prime (zero-indexed)
`Ù` | pops `a` | push uniquified a
`Ú` | pops `a` | push reverse uniquified a
`Û` | pops `a,b` | push a with leading b's trimmed off
`Ü` | pops `a,b` | push a with trailing b's trimmed off
`Ý` | pops `a` | push [0 .. a]
`Þ` | pops `a` | push float(a)
`ß` | pops `smallest` | element of list
`à` | pops `greatest` | element of list
`á` | pops `a` | push only letters of a
`â` | pops `a,(b)` | push cartesian product
`ã` | pops `a,b` | push a choose b (cartesian product repeat)
`ä` | pops `a,b` | push a sliced into b pieces
`å` | pops `a,b` | push a in b
`æ` | pops `a` | push powerset(a)
`ç` | pops `a` | push char a
`è` | pops `a,b` | push a[b]
`é` | pops `a` | push sorted a (key=length)
`ê` | pops `a` | push sorted_uniquified(a)
`ì` | pops `a,b` | push a.prepend(b)
`í` | pops `a` | push [reversed Q for Q in a] (short for €R)
`î` | pops `a` | push round_up(a)
`ï` | pops `a` | push int(a)
`ñ` | pops `a,b,c` | push a + b merged with c as merge character
`ò` | pops `a` | push inclusive round up a
`ó` | pops `a` | push inclusive round down a
`ô` | pops `a,b` | push a split in pieces of b
`ö` | pops `a,b` | push int(a, b)
`÷` | pops `a,b` | push a // b (integer division)
`ø` | pops `a` | push zipped a
`ù` | pops `a,b` | push a with elements of length b
`ú` | pops `a,b` | push a padded with b spaces in the front
`û` | pops `a` | push palindromized(a), 12345 becomes 123454321 (a + a[::-1][1:])
`ý` | pops `(a),b` | push b.join(a) if a is list, else b.join(stack)
`þ` | pops `a` | push only digits of a
`.å`| pops `a,b` | push a in b (vectorized)
`.A`| pops `a` | push acronymified a
`.b`| pops `a` | push letterified(a)
`.B`| pops `a` | push squarified(a)
`.c`| pops `a` | push centralized(a) focused to the left
`.C`| pops `a` | push centralized(a) focused to the right
`.D`| pops `a,b` | push b copies of a
`.e`| pops `a` | run with experimental python evaluation (does not work in safe mode)
`.E`| pops `a` | run with experimental batch evaluation (does not work in safe mode)
`.h`| pops `a,b` | bijectively convert a from base 10 to base b
`.H`| pops `a,b` | bijectively convert a from base b to base 10
`.j`| pops `a` | 0-indexed max_spaces.join(stack) grid (deprecated)
`.J`| pops `a` | 1-indexed max_spaces.join(stack) grid (deprecated)
`.l`| pops `a` | push is_lower(a)
`.L`| pops `a,b` | push levenshtein(a, b)
`.M`| pops `a` | push most frequent in a
`.m`| pops `a` | push least frequent in a
`.n`| pops `a,b` | push log_b(a)
`.N`| pops `a` | push hashed(a)
`.o`| pops `a,b` | push overlap(b) (deprecated)
`.O`| pops `a,b` | push connected_overlap(b) (deprecated)
`.p`| pops `a` | push prefixes(a)
`.R`| pops `a` | push random_pick(a)
`.r`| pops `a` | push random_shuffle(a)
`.s`| pops `a	` | push suffixes(a)
`.S`| pops `a,b` | push 1 if a > b, -1 if a < b, 0 if a == b 
`.u`| pops `a` | push is_upper(a) 
`.V`| pops `a` | run as 05AB1E code
`.w`| pops `a` | push a.readall() (internet access, doesn't work in safe mode) (returns 0 on error)
`.W`| pops `a` | wait a milliseconds
`.x`| pops `a,b` | push the element in a closest to b
`.:`| pops `a,b,c` | push a.replace(b, c)
`.;`| pops `a,b,c` | push a.replace_first(b, c)
`.²`| pops `a` | push log_2(a)
`.ï`| pops `a` | push is int(a)
`.¿`| pops `a,(b)` | push lcm(a, (b))
`.ˆ`| pops `a` | insert a into global array and after quit, print array[input_1]
`.^`| pops `a	` | insert a into global array with immediate sorting and after quit, print array[input_1]
`.ø`| pops `a,b` | surround a with b
`.×`| pops `a,b` | push the list a repeated b times
`.∞`| pops `a` | push intersected mirror a
`.¥`| pops `a` | push undelta a
`.ǝ`| pops `a` | print a to STDERR
`.∊`| pops `a` | push intersected vertical mirror a
`.Λ`| pops `a,b,c` | store a canvas with {a: num, b: filler, c: pattern} and push the string to the stack