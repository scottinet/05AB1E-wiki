## Commands

Command|Elements Popped|Description|
:-----:|:-------------:|-----------|
`ǝ` | `a,b,c` | insert **b** into **a** on location **c**
`ʒ` | `a` | filter **a**. Keep the elements where the result of the code is `1`: usage `ʒCODE}`
`α` | `a,b` | push absolute difference of **a** and **b**
`β` | `a,b` | push **a** converted from base **b** (arbitrary)
`γ` | `a` | push **a** split into chunks of consecutive equal elements
`δ` | `a,b` | get the next command, push double vectorized command
`ε` | `a` | apply each on **a**: usage `εCODE}`
`Δ` | `a` | repeat CODE until **a** doesn't change: usage `ΔCODE}`
`ζ` | `a,(b)` | push zipped **a** with filler **b** (standardized to space)
`η` | `a` | push the prefixes of **a**
`и` | `a,b` | push **a** n-repeat (list-multiply) **b**
`θ` | `a` | push `a[-1]`
`в` | `a,b` | push **a** converted to base **b** (arbitrary)
`м` | `a,b` | push **a** with elements that also occur in **b** removed
`н` | `a` | push `a[0]`
`Θ` | `a` | push 05AB1E truthified **a** (a == 1)
`Σ` | `a` | sort **a** by the result of code: usage `ΣCODE}`
`Ω` | `a` | push a random element of **a**
`≠` | `a` | push 05AB1E falsified **a** (a != 1)
`∊` | `a` | push vertically mirrored **a**
`∍` | `a,b` | push **a** extended/shortened to length **b**
`∞` | `a` | push mirrored **a**
`!` | `a,` | push the factorial of **a**
`#` | `a` | `if true: break/end` (used in infinite loops)
`#` | `a` | if **a** contains spaces, split by spaces.
`%` | `a,b` | modulo; push `(a % b)`
`&` | `a,b` | logical AND; push **a** AND **b**
`(` | `a` | push `-a`
`*` | `a,b` | multiplication; push `(a * b)`
`+` | `a,b` | addition; push `(a + b)`
`,` | `a` | print **a**
`-` | `a,b` | subtraction; push `(a - b)`
`/` | `a,b` | division; push `(a / b)`
`:` | `a,b,c` | `a.replace(b, c)` / infinite replacement
`;` | `a` | halve; push `a / 2`
`<` | `a` | decrement; push `a - 1`
`>` | `a` | increment; push `a + 1`
`?` | `a` | print **a**, with no newline
`@` | `a` | pop and push the element at index **a** in the stack (0-indexed)
`B` | `a,b` | push `base(a, b)`
`C` | `a` | push `int(a, 2)`
`D` | `a` | duplicate; push a, a
`F` | `a` | `for N in range(0, a) { }: F(commands)} / N = variable`
`G` | `a` | `for N in range(1, a) { }: F(commands)} / N = variable`
`H` | `a` | push `int(a, 16)`
`J` | `a` | push `''.join(a)` if **a** is list; Else, push `''.join(stack)`
`K` | `a,b` | push **a** without **b**'s
`L` | `a` | Inclusive range; push `[1 .. a]`
`O` | `a` | push total sum of **a** if **a** is list, else total sum of stack
`P` | `a` | push total product of **a** if **a** is list, else total product of stack
`Q` | `a,b` | push `a == b` (bool)
`R` | `a` | push **a** reversed
`S` | `a` | push all chars **a** separately
`U` | `a` | assign `X` to **a**
`V` | `a` | assign `Y` to **a**
`^` | `a,b` | push `a XOR b`
`_` | `a` | push negative bool
<code>`</code> | `a` | push all the items of **a** into the stack
`a` | `a` | push `is_alpha(a)`
`b` | `a` | push **a** in binary
`c` | `a,b` | Number of combinations; push `a nCr b`
`d` | `a` | push `is_number(a)`
`e` | `a,b` | Number of permutations; push `a nPr b`
`f` | `a` | push list of prime factors of **a** without duplicates
`g` | `a` | push the length of **a**
`h` | `a` | push `hex(a)`
`i` | `a` | if statement: `iTHEN}: if true { then }`
`j` | `a,b` | Same as `J`, with each substring right justified w/ a minimum length of **b**
`k` | `a,b` | push the index of **b** in **a** (0 indexed, -1 when not found)
`l` | `a` | push `lower_case(a)`
`m` | `a,b` | exponentiation; push `a ** b`
`n` | `a` | push `a**2`
`o` | `a` | push `2**a`
`p` | `a` | primality checking; push `isPrime(a)`
`s` | `a,b` | push `b,a`
`t` | `a` | square root; push `sqrt(a)`
`u` | `a` | uppercase; push `upper_case(a)`;
`v` | `a` | range loop - `for y in a` (y = string, N = index)
`x` | `a` | push **a**, `a * 2`
`z` | `a` | inverse; push `1 / a`
`}` | - | close a single if statement, loop, etc.
`]` | - | close all loops and if statements
`{` | `a` | sort; push `sorted a`
`~` | `a,b` | logical or; push `a OR b`
`Λ` | `a,b,c` | store **a** canvas with `{a: num, b: filler, c: pattern}` (todo: docs)
`‚` | `a,b` | push `[a, b]`
`ƒ` | `a` | push `for N in range(0, a + 1)`
`†` | `a,b` | push **a** with **b** filtered to the front
`‡` | `a,b,c` | push `a.transliterate(b -> c)`
`ˆ` | `a` | add to global array
`‰` | `a,b` | push `a divmod b`
`Š` | `a,b,c` | push `c,a,b`
`‹` | `a,b` | push `a < b`
`Œ` | `a` | substrings; push `substrings(a)`
`Ć` | `a` | push enclosed **a**: **a** + `a[0]`
`ƶ` | `a` | push lifted **a**, each element is multiplied by its index (1-indexed)
`Ā` | `a` | push truthified **a**
`–` | `a` | `if 1, print N` (used in loops)
`—` | `a` | `if 1, print y` (used in loops)
`˜` | `a` | push deep flattened **a**
`™` | `a` | push `title_cased(a)`
`š` | `a` | push `switch_cased(a)`
`›` | `a,b` | push `a > b`
`œ` | `a` | permutations; push `permutations(a)`
`ć` | `a` | push head_extracted **a**: `a[1:], a[0]`
`Ÿ` | `(a,)b` | inclusive binary range; push [a, ..., b] if **b** is not a list, else push [b[0],...,b[1],...,b[n]]
`¡` | `a,b` | push `a.split(b)` 
`¢` | `a,b` | push `a.count(b)`
`£` | `a,b` | push `a[0:b]`
`¥` | `a` | push the deltas of **a**
`¦` | `a` | tail; push `a[1:]`
`§` | `a` | push `str(a)`
`¨` | `a` | head; push `a[0:-1]`
`ª` | `a` | push `sentence_cased(a)`
`«` | `a,b` | push `merged(a,b)` if both are lists, else push `concatenated(a, b)`
`°` | `a` | push `10**a`
`±` | `a` | bitwise not; push `~a`
`µ` | `a` | `while counter_variable != a, do...`
`·` | `a` | double; push `2 * a`
`¸` | `a` | listify; push `[a]`
`»` | `(a)` | if `(a)` is **a** list, join it by newlines, else join stack by newlines
`½` | `a,` | if 1, then increment the `counter_variable`
`¿` | `(a,)b` | push `gcd(b)` if **b** is list, else push `gcd([b, a])`
`À` | `a` | push **a** rotated 1 left
`Á` | `a` | push **a** rotated 1 right
`Â` | `a` | push bifurcated  **a**
`Ã` | `a,b` | push `a.keep(b)`
`Ä` | `a` | absolute value; push `abs(a)`
`Æ` | `a` | push reduced substraction **a**
`Ç` | `a` | ord; push ASCII value of **a**
`È` | `a` | even; push `a % 2 == 0`
`É` | `a` | odd; push `a % 2 == 1`
`Ê` | `a,b` | push `a != b`
`Ë` | `a` | push 1 if all elements are equal else 0
`Ì` | `a` | push `a + 2`
`Í` | `a` | push `a - 2`
`Ï` | `a,b` | push the elements from **a** at which the same index at **b** is 1
`Ñ` | `a` | divisors; push `divisors(a)`
`Ò` | `a` | push the list of prime factors of **a** (with duplicates)
`Ó` | `a` | push the list of exponents of prime factors (`2^a`, `3^b`, `5^c`, `7^d`, etc.)
`Ô` | `a` | push connected uniquified **a**
`Õ` | `a` | totient; push `euler_totient(a)`
`Ö` | `a,b` | divisible; push `a % b == 0`
`×` | `a,b` | push `a × b` (strings)
`Ø` | `a` | push **a** th prime (zero-indexed)
`Ù` | `a` | push uniquified **a**
`Ú` | `a` | push reverse uniquified **a**
`Û` | `a,b` | push **a** with leading **b**'s trimmed off
`Ü` | `a,b` | push **a** with trailing **b**'s trimmed off
`Ý` | `a` | Inclusive 0-based range; push `[0 .. a]`
`Þ` | `a` | push stringified `float(a)`
`ß` | `a` | extract smallest element of list
`à` | `a` | extract greatest element of list
`á` | `a` | push the letters of **a**
`â` | `a,b` | push cartesian product
`ã` | `(a,)b` | push cartesian product of `b.repeat(2)` if **b** is list, else cartesian product of `a.repeat(b)`
`ä` | `a,b` | push **a** sliced into **b** pieces
`å` | `a,b` | push `b in a`
`æ` | `a` | push `powerset(a)`
`ç` | `a` | push char **a**
`è` | `a,b` | push `a[b]`
`é` | `a` | push sorted **a** by length
`ê` | `a` | push `sorted_uniquified(a)`
`ì` | `a,b` | push `a.prepend(b)`
`í` | `a` | push `[reversed Q for Q in a]` (short for `€R`)
`î` | `a` | push `round_up(a)`
`ï` | `a` | push `int(a)`
`ñ` | `a,b,c` | push `a + b` merged with **c** as merge character
`ò` | `a` | push `round_nearest(a)` (bankers rounding)
`ó` | `a` | push `round_down(a)`
`ô` | `a,b` | push **a** split in pieces of **b**
`ö` | `a,b` | push `int(a, b)`
`÷` | `a,b` | integer division; push `a // b`
`ø` | `(a,)b` | push `zip(b)` if **b** is list, else `zip(a,b)`
`ù` | `a,b` | push **a** with elements of length **b**
`ú` | `a,b` | push **a** padded with **b** spaces in the front
`û` | `a` | push `palindromized(a)`, `12345` becomes `123454321` (`a + a[::-1][1:]`)
`ý` | `(a),b` | push `b.join(a)` if **a** is a list, else `b.join(stack)`
`þ` | `a` | push the digits of **a**
`.å`| `a,b` | push `a in b` (vectorized)
`.A`| `a` | push acronymified **a**
`.b`| `a` | push `letterified(a)`
`.B`| `a` | push `squarified(a)`
`.c`| `a` | push `centralized(a)` focused to the left
`.C`| `a` | push `centralized(a)` focused to the right
`.D`| `a,b` | push **b** copies of **a**
`.e`| `a` | run with experimental python evaluation (does not work in safe mode)
`.E`| `a` | run with experimental batch evaluation (does not work in safe mode)
`.h`| `a,b` | bijectively convert **a** from base 10 to base **b**
`.H`| `a,b` | bijectively convert **a** from base **b** to base 10
`.j`| `a` | 0-indexed `max_spaces.join(stack) grid` (deprecated)
`.J`| `a` | 1-indexed `max_spaces.join(stack) grid` (deprecated)
`.l`| `a` | push `is_lower(a)`
`.L`| `a,b` | Levenshtein distance; push `levenshtein(a, b)`
`.M`| `a` | push most frequent element in **a**
`.m`| `a` | push least frequent element in **a**
`.n`| `a,b` | logarithm; push `log_b(a)`
`.N`| `a` | push `hashed(a)`
`.o`| `a,b` | push `overlap(b)` (deprecated)
`.O`| `a,b` | push `connected_overlap(b)` (deprecated)
`.p`| `a` | prefixes; push `prefixes(a)`
`.R`| `a` | random element; push `random_pick(a)`
`.r`| `a` | shuffle; push `random_shuffle(a)`
`.s`| `a` | suffixes; push `suffixes(a)`
`.S`| `a,b` | push 1 if `a > b`, -1 if `a < b`, 0 if `a == b` 
`.u`| `a` | push `is_upper(a)`
`.V`| `a` | run as 05AB1E code
`.w`| `a` | push `a.readall()` (internet access, doesn't work in safe mode) (returns 0 on error)
`.W`| `a` | wait **a** milliseconds
`.x`| `a,b` | push the element in **a** closest to **b**
`.:`| `a,b,c` | push `a.replace(b, c)`
`.;`| `a,b,c` | push `a.replace_first(b, c)`
`.²`| `a` | log base 2; push `log_2(a)`
`.ï`| `a` | check if a is an integer; push `is int(a)`
`.¿`| `(a,)b` | lcm (hcf); push `lcm(b)` if **b** is list, else push `lcm(b, a)`
`.ˆ`| `a` | insert **a** into global array and after quit, print `array[input_1]`
`.^`| `a` | insert **a** into global array with immediate sorting and after quit, print `array[input_1]`
`.ø`| `a,b` | surround **a** with **b**
`.×`| `a,b` | push the list **a** repeated **b** times
`.∞`| `a` | push intersected mirror **a**
`.¥`| `a` | push undelta **a**
`.ǝ`| `a` | print **a** to STDERR
`.∊`| `a` | push intersected vertical mirror **a**
`.Λ`| `a,b,c` | store **a** canvas with `{a: num, b: filler, c: pattern}` and push the string to the stack
`.Ø` | `a` | push 0-indexed number of the greatest prime ≤ **a**
`.ò` | `a,b` | round **a** with **b** digits precision (bankers rounding)
`т`  | - | push 100
`₁`  | - | push 256
`₂`  | - | push 26
`₃`  | - | push 95
`₄`  | - | push 1000
`₆`  | - | 
`"`  | - | start/end string literal
`$`  | - | push 1 and input (used for sequences)
`'`  | - | push char ( 'a pushes "a" )
`)`  | - | wrap total stack to an array
`.`  | - | two char functions
`0`  | - | numeric literal
`1`  | - | numeric literal
`2`  | - | numeric literal
`3`  | - | numeric literal
`4`  | - | numeric literal
`5`  | - | numeric literal
`6`  | - | numeric literal
`7`  | - | numeric literal
`8`  | - | numeric literal
`9`  | - | numeric literal
`=`  | - | print last item
`A`  | - | push 'abcdefghijklmnopqrstuvwxyz'
`E`  | - | push eval(input())
`I`  | - | push input()
`M`  | - | push the largest number in the stack
`N`  | - | reserved for variables
`T`  | - | push 10
`W`  | - | push min(a) without popping
`X`  | - | integer variable
`Y`  | - | integer variable
`Z`  | - | push max(a) without popping
`[`  | - | infinite loop start
`\`  | - | delete last item
`]`  | - | infinite loop end
`q`  | - | terminates the program
`r`  | - | reverse stack
`w`  | - | wait one second
`y`  | - | push string variable (used in mapping loops)
`\|`  | - | push the rest of input as an array with strings
`}`  | - | used to close if statements, loops, etc.
`Ƶ`  | - | convert the next char from base 255 to base 10 and add 101
`€`  | - | Map; Apply the next command to each element in the list.
`„`  | - | 2 char string / can also be used for 2 compressed strings
`…`  | - | 3 char string / can also be used for 3 compressed strings
`Ž`  | - | break if stack is empty
`‘`  | - | for compressed strings (upper)
`’`  | - | for compressed strings (no implicit space)
`“`  | - | for compressed strings (normal)
`”`  | - | for compressed strings (title)
`•`  | - | start/end a 1-9 char compressed string
`ā`  | - | get a; push `range(1, len(a) + 1)`
`¤`  | - | get a; push `tail(a)`
`©`  | - | store a in register_c without popping
`¬`  | - | get a; push `head(a)`
`®`  | - | push the last item from register_c
`¯`  | - | push global array
`²`  | - | push the second item from the input history
`³`  | - | push the third item from the input history
`´`  | - | clear global array
`¶`  | - | push newline character
`¹`  | - | push the first item from the input history
`º`  | - | push `len(stack) > 0`
`¼`  | - | counter_variable += 1
`¾`  | - | push counter_variable
`Å`  | - | list commands
`Î`  | - | push 0 and input
`Ð`  | - | triplicate top of stack (pop **a**, push **a**, push **a**, push **a**)
`ë`  | - | else statement
`ð`  | - | push a space character
`õ`  | - | push empty string
`ü`  | - | pairwise command (vectorizes if the first element is a list)
`ÿ`  | - | used for string interpolation, pop **a** and replace `ÿ` with `str(a)`
`.€` | - | debug printer
`.ä` | - | debug printer
`.0` | - | throw a division by zero error
`.g` | - | push length of stack
`.«` | - | foldr; folds a dyadic command between each element in a list from right to left
`.»` | - | foldl; folds a dyadic command between each element in a list from right to left with opposite right/left operands
`.À` | - | rotate stack 1 left
`.Á` | - | rotate stack 1 right
`.•` | - | decompress a base 255 alphabet based string

## `ž` - Commands

Command|Description|
-------|-----------|
`ža` | push current hours
`žb` | push current minutes
`žc` | push current seconds
`žd` | push current microseconds
`že` | push current day
`žf` | push current month
`žg` | push current year
`žh` | push `[0-9]`
`ži` | push `[a-zA-Z]`
`žj` | push `[a-zA-Z0-9_]`
`žk` | push `[z-aZ-A]`
`žl` | push `[z-aZ-A9-0_]`
`žm` | push `[9-0]`
`žn` | push `[A-Za-z]`
`žo` | push `[Z-Az-a]`
`žp` | push `[Z-A]`
`žq` | push `pi`
`žr` | push `e`
`žs` | pop **a**, push `pi` to **a** digits (max. 100000)
`žt` | pop **a**, push `e` to **a** digits (max. 10000)
`žu` | push `()<>[]{}`
`žv` | push `16`
`žw` | push `32`
`žx` | push `64`
`žy` | push `128`
`žz` | push `256`
`žA` | push `512`
`žB` | push `1024`
`žC` | push `2048`
`žD` | push `4096`
`žE` | push `8192`
`žF` | push `16384`
`žG` | push `32768`
`žH` | push `65536`
`žI` | push `2147483648`
`žJ` | push `4294967296`
`žK` | push `[a-zA-Z0-9]`
`žL` | push `[z-aZ-A9-0]`
`žM` | push `"aeiou"`
`žN` | push `"bcdfghjklmnpqrstvwxyz"`
`žO` | push `"aeiouy"`
`žP` | push `"bcdfghjklmnpqrstvwxz"`
`žQ` | push printable ASCII character set (32-128)
`žR` | push `"ABC"`
