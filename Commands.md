Command|Elements Popped|Description|
-------|---------------|-----------|
`ǝ` | `a,b,c` | insert **`b`** into **`a`** on location **`c`** 
`ʒ` | `a` | filter **`a`** when the result of **`c`** ode equals 1: usage ʒCODE}
`α` | `a,b` | push **`a`** **`b`** solute difference of **`a`** **`a`** nd **`b`** 
`β` | `a,b` | push **`a`** **`c`** onverted from **`b`** ase **`b`** (arbitrary)
`γ` | `a` | push **`a`** split into **`c`** hunks of **`c`** onsecutive equal elements
`δ` | `a,b` | get the next **`c`** ommand, push double vectorized **`c`** ommand
`ε` | `a` | **`a`** pply each on **`a`** : usage εCODE}
`ζ` | `a,(b)` | push zipped **`a`** with filler **`b`** (standardized to space)
`η` | `a` | push prefixes(a)
`θ` | `a` | push **`a`** [-1]
`в` | `a,b` | push **`a`** **`c`** onverted to **`b`** ase **`b`** (arbitrary)
`м` | `a,b` | push **`a`** .remove(all elements of **`b`** )
`н` | `a` | push **`a`** [0]
`Θ` | `a` | push 05AB1E truthified **`a`** (a == 1)
`Σ` | `a` | sort **`a`** **`b`** y the result of **`c`** ode: usage ΣCODE}
`Ω` | `a` | push random_pick(a)
`≠` | `a` | push 05AB1E falsified **`a`** (a != 1)
`∊` | `a` | push vertically mirrored **`a`** 
`∍` | `a,b` | push **`a`** extended/shortened to length **`b`** 
`∞` | `a` | push mirrored **`a`** 
`!` | `a,` | push factorial(a)
`#` | `a` | if true: **`b`** reak/end (used in infinite loops)
`#` | `a` | if **`c`** ontains spaces, split on spaces
`%` | `a,b` | push (a % **`b`** )
`&` | `a,b` | push **`a`** AND **`b`** 
`(` | `a` | push -a
`*` | `a,b` | push (a * **`b`** )
`+` | `a,b` | push (a + **`b`** )
`,` | `a` | print(a)
`-` | `a,b` | push (a - **`b`** )
`/` | `a,b` | push (a / **`b`** )
`:` | `a,b,c` | **`a`** .replace(b, **`c`** ) / infinite replacement
`;` | `a` | push **`a`** / 2
`<` | `a` | push **`a`** - 1
`>` | `a` | push **`a`** + 1
`?` | `a` | print **`a`** no newline
`@` | `a` | pop **`a`** nd push the element **`a`** t index **`a`** in the stack (leftmost element = index 0)
`B` | `a,b` | push **`b`** ase(a, **`b`** )
`C` | `a` | push int(a, 2)
`D` | `a` | push **`a`** , **`a`** 
`F` | `a` | for N in range(0, **`a`** ) { }: F(commands)} / N = variable
`G` | `a` | for N in range(1, **`a`** ) { }: F(commands)} / N = variable
`H` | `a` | push int(a, 16)
`J` | `a` | push ''.join(a) if **`a`** is list / if not, then push ''.join(stack)
`K` | `a,b` | push **`a`** with no **`b`** 's
`L` | `a` | push [1 .. **`a`** ]
`O` | `a` | push total sum (only on lists)
`P` | `a` | push total product (only on lists)
`Q` | `a,b` | push **`a`** == **`b`** (bool)
`R` | `a` | push reversed(a)
`S` | `a` | push **`a`** ll **`c`** hars **`a`** seperate
`U` | `a` | **`a`** ssign X to **`a`** 
`V` | `a` | **`a`** ssign Y to **`a`** 
`^` | `a,b` | push **`a`** XOR **`b`** 
`_` | `a` | push negative **`b`** ool
``` | `a` | push **`a`** ll the items of **`a`** into the stack
`a` | `a` | push is_alpha(a)
`b` | `a` | push **`b`** in(a)
`c` | `a,b` | push **`a`** nCr **`b`** 
`d` | `a` | push is_number(a)
`e` | `a,b` | push **`a`** nPr **`b`** 
`f` | `a` | push list of prime factors (no duplicates)
`g` | `a` | push length of **`a`** 
`h` | `a` | push hex(a)
`i` | `a` | if statement: iTHEN}: if true { then }
`j` | `a` | max_a_spaces.join(stack)
`k` | `a,b` | push 0-indexed index of **`b`** in **`a`** (-1 when not found)
`l` | `a` | push lower_case(a)
`m` | `a,b` | push **`a`** **b
`n` | `a` | push **`a`** **2
`o` | `a` | push 2**a
`p` | `a` | push isPrime(a)
`s` | `a,b` | push **`b`** ,a
`t` | `a` | push sqrt(a)
`u` | `a` | push upper_case(a)
`v` | `a` | range loop: for y in **`a`** (y = string, N = index)
`x` | `a` | push **`a`** , **`a`** * 2
`z` | `a` | push 1 / **`a`** 
`{` | `a` | push sorted **`a`** 
`~` | `a,b` | push **`a`** OR **`b`** 
`Λ` | `a,b,c` | store **`a`** **`c`** anvas with {a: num, **`b`** : filler, **`c`** : pattern} (todo: docs)
`‚` | `a,b` | push [a, **`b`** ]
`ƒ` | `a` | push for N in range(0, **`a`** + 1)
`†` | `a,b` | push **`a`** with **`b`** filtered to the front
`‡` | `a,b,c` | push **`a`** .transliterate(b -> **`c`** )
`ˆ` | `a` | **`a`** dd to global **`a`** rray
`‰` | `a,b` | push **`a`** divmod **`b`** 
`Š` | `a,b,c` | push **`c`** ,a,b
`‹` | `a,b` | push **`a`** < **`b`** 
`Œ` | `a` | push substrings(a)
`Ć` | `a` | push enclosed **`a`** : **`a`** + **`a`** [0]
`ƶ` | `a` | push lifted **`a`** , each element is multiplied **`b`** y its index (1-indexed)
`Ā` | `a` | push truthified **`a`** 
`–` | `a` | if 1, print N (used in loops)
`—` | `a` | if 1, print y (used in loops)
`˜` | `a` | push deep flattened **`a`** 
`™` | `a` | push title_cased(a)
`š` | `a` | push switch_cased(a)
`›` | `a,b` | push **`a`** > **`b`** 
`œ` | `a` | push permutations(a)
`ć` | `a` | push head_extracted **`a`** : **`a`** [1:], **`a`** [0] 
`Ÿ` | `a,b` | push [a, ..., **`b`** ]
`¡` | `a,b` | push **`a`** .split(b)  
`¢` | `a,b` | push **`a`** .count(b)
`£` | `a,b` | push **`a`** [0:b]
`¥` | `a` | push delta's **`a`** 
`¦` | `a` | push **`a`** [1:]
`§` | `a` | push str(a)
`¨` | `a` | push **`a`** [0:-1]
`ª` | `a` | push sentence_cased(a)
`«` | `a,b` | push **`c`** oncatenated(a, **`b`** )
`°` | `a` | push 10 ** **`a`** 
`±` | `a` | push **`b`** itwise not **`a`** 
`µ` | `a` | while **`c`** ounter_variable != **`a`** , do...
`·` | `a` | push 2 * **`a`** 
`¸` | `a` | push [a]
`»` | `(a)` | if list, join list **`b`** y newlines, else join stack **`b`** y newlines
`½` | `a,` | if 1, then **`c`** ounter_variable += 1
`¿` | `a` | push gcd(a)
`À` | `a` | push **`a`** rotated 1 left
`Á` | `a` | push **`a`** rotated 1 right
`Â` | `a` | push **`b`** ifurcated **`a`** 
`Ã` | `a,b` | push **`a`** .keep(b)
`Ä` | `a` | push **`a`** **`b`** s(a)
`Æ` | `a` | push reduced substraction **`a`** 
`Ç` | `a` | push ASCII value of **`a`** 
`È` | `a` | push **`a`** % 2 == 0 (is even)
`É` | `a` | push **`a`** % 2 == 1 (is uneven)
`Ê` | `a,b` | push **`a`** != **`b`** 
`Ë` | `a` | push 1 if **`a`** ll equal else 0
`Ì` | `a` | push **`a`** + 2
`Í` | `a` | push **`a`** - 2
`Ï` | `a,b` | push the elements from **`a`** **`a`** t which the same index **`a`** t **`b`** is 1
`Ñ` | `a` | push divisors(a)
`Ò` | `a` | push list of prime factors (with duplicates)
`Ó` | `a` | push list of exponents of prime factors (2^a, 3^b, 5^c, 7^d, etc.)
`Ô` | `a` | push **`c`** onnected uniquified **`a`** 
`Õ` | `a` | push euler_totient(a)
`Ö` | `a,b` | push **`a`** % **`b`** == 0
`×` | `a,b` | push **`a`** × **`b`** (strings)
`Ø` | `a` | push **`a`** th prime (zero-indexed)
`Ù` | `a` | push uniquified **`a`** 
`Ú` | `a` | push reverse uniquified **`a`** 
`Û` | `a,b` | push **`a`** with leading **`b`** 's trimmed off
`Ü` | `a,b` | push **`a`** with trailing **`b`** 's trimmed off
`Ý` | `a` | push [0 .. **`a`** ]
`Þ` | `a` | push float(a)
`ß` | `smallest` | element of list
`à` | `greatest` | element of list
`á` | `a` | push only letters of **`a`** 
`â` | `a,(b)` | push **`c`** artesian product
`ã` | `a,b` | push **`a`** **`c`** hoose **`b`** (cartesian product repeat)
`ä` | `a,b` | push **`a`** sliced into **`b`** pieces
`å` | `a,b` | push **`a`** in **`b`** 
`æ` | `a` | push powerset(a)
`ç` | `a` | push **`c`** har **`a`** 
`è` | `a,b` | push **`a`** [b]
`é` | `a` | push sorted **`a`** (key=length)
`ê` | `a` | push sorted_uniquified(a)
`ì` | `a,b` | push **`a`** .prepend(b)
`í` | `a` | push [reversed Q for Q in **`a`** ] (short for €R)
`î` | `a` | push round_up(a)
`ï` | `a` | push int(a)
`ñ` | `a,b,c` | push **`a`** + **`b`** merged with **`c`** **`a`** s merge **`c`** haracter
`ò` | `a` | push inclusive round up **`a`** 
`ó` | `a` | push inclusive round down **`a`** 
`ô` | `a,b` | push **`a`** split in pieces of **`b`** 
`ö` | `a,b` | push int(a, **`b`** )
`÷` | `a,b` | push **`a`** // **`b`** (integer division)
`ø` | `a` | push zipped **`a`** 
`ù` | `a,b` | push **`a`** with elements of length **`b`** 
`ú` | `a,b` | push **`a`** padded with **`b`** spaces in the front
`û` | `a` | push palindromized(a), 12345 **`b`** ecomes 123454321 (a + **`a`** [::-1][1:])
`ý` | `(a),b` | push **`b`** .join(a) if **`a`** is list, else **`b`** .join(stack)
`þ` | `a` | push only digits of **`a`** 
`.å`| `a,b` | push **`a`** in **`b`** (vectorized)
`.A`| `a` | push **`a`** **`c`** ronymified **`a`** 
`.b`| `a` | push letterified(a)
`.B`| `a` | push squarified(a)
`.c`| `a` | push **`c`** entralized(a) focused to the left
`.C`| `a` | push **`c`** entralized(a) focused to the right
`.D`| `a,b` | push **`b`** **`c`** opies of **`a`** 
`.e`| `a` | run with experimental python evaluation (does not work in safe mode)
`.E`| `a` | run with experimental **`b`** atch evaluation (does not work in safe mode)
`.h`| `a,b` | **`b`** ijectively **`c`** onvert **`a`** from **`b`** ase 10 to **`b`** ase **`b`** 
`.H`| `a,b` | **`b`** ijectively **`c`** onvert **`a`** from **`b`** ase **`b`** to **`b`** ase 10
`.j`| `a` | 0-indexed max_spaces.join(stack) grid (deprecated)
`.J`| `a` | 1-indexed max_spaces.join(stack) grid (deprecated)
`.l`| `a` | push is_lower(a)
`.L`| `a,b` | push levenshtein(a, **`b`** )
`.M`| `a` | push most frequent in **`a`** 
`.m`| `a` | push least frequent in **`a`** 
`.n`| `a,b` | push log_b(a)
`.N`| `a` | push hashed(a)
`.o`| `a,b` | push overlap(b) (deprecated)
`.O`| `a,b` | push **`c`** onnected_overlap(b) (deprecated)
`.p`| `a` | push prefixes(a)
`.R`| `a` | push random_pick(a)
`.r`| `a` | push random_shuffle(a)
`.s`| `a	` | push suffixes(a)
`.S`| `a,b` | push 1 if **`a`** > **`b`** , -1 if **`a`** < **`b`** , 0 if **`a`** == **`b`** 
`.u`| `a` | push is_upper(a) 
`.V`| `a` | run **`a`** s 05AB1E **`c`** ode
`.w`| `a` | push **`a`** .readall() (internet **`a`** **`c`** cess, doesn't work in safe mode) (returns 0 on error)
`.W`| `a` | wait **`a`** milliseconds
`.x`| `a,b` | push the element in **`a`** **`c`** losest to **`b`** 
`.:`| `a,b,c` | push **`a`** .replace(b, **`c`** )
`.;`| `a,b,c` | push **`a`** .replace_first(b, **`c`** )
`.²`| `a` | push log_2(a)
`.ï`| `a` | push is int(a)
`.¿`| `a,(b)` | push lcm(a, (b))
`.ˆ`| `a` | insert **`a`** into global **`a`** rray **`a`** nd **`a`** fter quit, print **`a`** rray[input_1]
`.^`| `a	` | insert **`a`** into global **`a`** rray with immediate sorting **`a`** nd **`a`** fter quit, print **`a`** rray[input_1]
`.ø`| `a,b` | surround **`a`** with **`b`** 
`.×`| `a,b` | push the list **`a`** repeated **`b`** times
`.∞`| `a` | push intersected mirror **`a`** 
`.¥`| `a` | push undelta **`a`** 
`.ǝ`| `a` | print **`a`** to STDERR
`.∊`| `a` | push intersected vertical mirror **`a`** 
`.Λ`| `a,b,c` | store **`a`** **`c`** anvas with {a: num, **`b`** : filler, **`c`** : pattern} **`a`** nd push the string to the stack