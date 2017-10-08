Command|Elements Popped|Description|
-------|---------------|-----------|
`ǝ` | `a,b,c` | insert **`b`** into **`a`** on location **`c`**
`ʒ` | `a` | filter **`a`** when the result of code equals 1: usage ʒCODE}
`α` | `a,b` | push absolute difference of **`a`** and **`b`**
`β` | `a,b` | push **`a`** converted from base **`b`** (arbitrary)
`γ` | `a` | push **`a`** split into chunks of consecutive equal elements
`δ` | `a,b` | get the next command, push double vectorized command
`ε` | `a` | apply each on **`a`**: usage **`εCODE}`**
`ζ` | `a,(b)` | push zipped **`a`** with filler **`b`** (standardized to space)
`η` | `a` | push the prefixes of **`a`**
`θ` | `a` | push **`a[-1]`**
`в` | `a,b` | push **`a`** converted to base **`b`** (arbitrary)
`м` | `a,b` | push **`a`** with elements that also occur in **`b`** removed
`н` | `a` | push **`a[0]`**
`Θ` | `a` | push 05AB1E truthified **`a`** (a == 1)
`Σ` | `a` | sort **`a`** by the result of code: usage `ΣCODE}`
`Ω` | `a` | push a random element of **a**
`≠` | `a` | push 05AB1E falsified **`a`** (a != 1)
`∊` | `a` | push vertically mirrored **`a`**
`∍` | `a,b` | push **`a`** extended/shortened to length **`b`**
`∞` | `a` | push mirrored **`a`**
`!` | `a,` | push the factorial of **`a`**
`#` | `a` | `if true: break/end` (used in infinite loops)
`#` | `a` | if **`a`** contains spaces, split by spaces.
`%` | `a,b` | modulo; push **`(a % b)`**
`&` | `a,b` | logical AND; push **`a`** AND **`b`**
`(` | `a` | push **`-a`**
`*` | `a,b` | multiplication; push **`(a * b)`**
`+` | `a,b` | addition; push **`(a + b)`**
`,` | `a` | print **`a`**
`-` | `a,b` | subtraction; push **`(a - b)`**
`/` | `a,b` | division; push **`(a / b)`**
`:` | `a,b,c` | a.replace(b, c) / infinite replacement
`;` | `a` | halve; push **`a / 2`**
`<` | `a` | decrement; push **`a - 1`**
`>` | `a` | increment; push **`a + 1`**
`?` | `a` | print **`a`**, with no newline
`@` | `a` | pop and push the element at index **`a`** in the stack (0-indexed)
`B` | `a,b` | push **`base(a, b)`**
`C` | `a` | push **`int(a, 2)`**
`D` | `a` | duplicate; push a, a
`F` | `a` | **`for N in range(0, a) { }: F(commands)} / N = variable`**
`G` | `a` | **`for N in range(1, a) { }: F(commands)} / N = variable`**
`H` | `a` | push **`int(a, 16)`**
`J` | `a` | push **`''.join(a)`** if **`a`** is list; Else, push **`''.join(stack)`**
`K` | `a,b` | push **`a`** without **`b`**'s
`L` | `a` | Inclusive range; push **`[1 .. a]`**
`O` | `a` | push total sum (only on lists)
`P` | `a` | push total product (only on lists)
`Q` | `a,b` | push **`a == b`** (bool)
`R` | `a` | push **`a`** reversed
`S` | `a` | push all chars **`a`** separately
`U` | `a` | assign **`X`** to **`a`**
`V` | `a` | assign **`Y`** to **`a`**
`^` | `a,b` | push **`a XOR b`**
`_` | `a` | push negative bool
``` | `a` | push all the items of **`a`** into the stack
`a` | `a` | push **`is_alpha(a)`**
`b` | `a` | push **`a`** in binary
`c` | `a,b` | Number of combinations; push **`a`** nCr b
`d` | `a` | push `is_number(a)`
`e` | `a,b` | Number of permutations; push **`a`** nPr b
`f` | `a` | push list of prime factors of **`a`** without duplicates
`g` | `a` | push the length of **`a`**
`h` | `a` | push **`hex(a)`**
`i` | `a` | if statement: **`iTHEN}: if true { then }`**
`j` | `a` | **`max_a_spaces.join(stack)`**
`k` | `a,b` | push the index of **`b`** in **`a`** (0 indexed, -1 when not found)
`l` | `a` | push **`lower_case(a)`**
`m` | `a,b` | Exponentiation; push **`a ** b`**
`n` | `a` | push **`a ** 2`**
`o` | `a` | push **`2 ** a`**
`p` | `a` | primality checking; push **`isPrime(a)`**
`s` | `a,b` | push **`b,a`**
`t` | `a` | square root; push **`sqrt(a)`**
`u` | `a` | uppercase; push **`upper_case(a)`**;
`v` | `a` | range loop - **`for y in a`** (y = string, N = index)
`x` | `a` | push **`a`**, **`a * 2`**
`z` | `a` | inverse; push **`1 / a`**
`{` | `a` | sort; push **`sorted a`**
`~` | `a,b` | logical or; push **`a OR b`**
`Λ` | `a,b,c` | store **`a`** canvas with **`{a: num, b: filler, c: pattern}`** (todo: docs)
`‚` | `a,b` | push **`[a, b]`**
`ƒ` | `a` | push **`for N in range(0, **`a`** + 1)`**
`†` | `a,b` | push **`a`** with **`b`** filtered to the front
`‡` | `a,b,c` | push **`a.transliterate(b -> c)`**
`ˆ` | `a` | add to global array
`‰` | `a,b` | push **`a divmod b`**
`Š` | `a,b,c` | push **`c,a,b`**
`‹` | `a,b` | push **`a < b`**
`Œ` | `a` | substrings; push **`substrings(a)`**
`Ć` | `a` | push enclosed **`a`**: **`a`** + **`a[0]`**
`ƶ` | `a` | push lifted **`a`**, each element is multiplied by its index (1-indexed)
`Ā` | `a` | push truthified **`a`**
`–` | `a` | **`if 1, print N`** (used in loops)
`—` | `a` | **`if 1, print y`** (used in loops)
`˜` | `a` | push deep flattened **`a`**
`™` | `a` | push **`title_cased(a)`**
`š` | `a` | push **`switch_cased(a)`**
`›` | `a,b` | push **`a > b`**
`œ` | `a` | permutations; push **`permutations(a)`**
`ć` | `a` | push head_extracted **`a`**: **`a[1:], a[0]`**
`Ÿ` | `a,b` | inclusive binary range; push **`[a, ..., b]`**
`¡` | `a,b` | push **`a.split(b)`** 
`¢` | `a,b` | push **`a.count(b)`**
`£` | `a,b` | push **`a[0:b]`**
`¥` | `a` | push the deltas of **`a`**
`¦` | `a` | tail; push **`a[1:]`**
`§` | `a` | push **`str(a)`**
`¨` | `a` | head; push **`a[0:-1]`**
`ª` | `a` | push **`sentence_cased(a)`**
`«` | `a,b` | push **`concatenated(a, b)`**
`°` | `a` | push **`10 ** a`**
`±` | `a` | bitwise not; push **`~a`**
`µ` | `a` | `while counter_variable != a, do...`
`·` | `a` | double; push **`2 * a`**
`¸` | `a` | wrap; push **`[a]`**