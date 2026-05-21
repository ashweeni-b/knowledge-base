### Conventional Commits

Standard for writing commits

*Structure:*

\<type\> (\<scope\>): \<short-description-of-commit\> <br />
[optional_body] <br />
[optional_footer] 

*Example:*

feat (pointers): add pointer arithmetic examples <br />

Explored pointer increment, decrement and address calculation. <br />
Understood how pointer moves by data types size not 1 byte. <br />

Closes \#12

*Commit types:*

| Type | Use for |
| -------- | ------- |
| feat | New code, new concept learned |
| fix | Bug fix, logical error corrected |
| docs | README, notes, comments |
| refactor | Same logic, cleaner code |
| style | Formatting, indentation, no logic change |
| test | Adding or fixing test cases |
| chore | Folder structure, config, setup |
| perf | Performance improvement |
| revert | Undoing a previous commit |

---