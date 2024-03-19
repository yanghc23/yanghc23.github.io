元字符（Metacharacters）是正则表达式中的特殊字符，这些字符在正则表达式中具有特殊含义。下面是一些常见的元字符：

1. `.`：匹配任何单个字符，除了换行符。
2. `^`：匹配字符串的开头。
3. `$`：匹配字符串的结尾。
4. `*`：匹配前面的表达式零次或多次。
5. `+`：匹配前面的表达式一次或多次。
6. `?`：匹配前面的表达式零次或一次。
7. `[]`：匹配括号内的任意一个字符。例如，`[abc]`将匹配字符'a'，'b'或'c'。
8. `[a-z]`：匹配字母'a'到'z'之间的任意一个字符。
9. `[^]`：匹配不在括号内的任意一个字符。例如，`[^abc]`将匹配任何不是字符'a'，'b'或'c'的字符。
10. `()`：定义子组。

可以使用 `\` (反斜线)字符来转义元字符以匹配它们的字面值。例如，如果字符串中包含字符 `.`，则需要使用 `\.` 来匹配实际字符 '.'。

| Metacharacter | Meaning             |
| ------------- | ------------------- |
| .             | Any Character       |
| \\w           | A Word              |
| \\W           | Not a Wold          |
| \\d           | A Digit             |
| \\D           | Not a Digit         |
| \\s           | Whitespace          |
| \\S           | Not Whitespace      |
|               | A Set of Characters |
|               | Negation of Set     |


## Find

```bash
find [directory] -name [filename]
```

-   `[directory]` is the directory where you want to begin the search. This can be any directory in your system. If you want to search the *entire system*, you can use `/` as the directory. If you want to search just your *home directory*, you can use `~`. And if you want to search the *current directory*, you can use `.`.
    
-   `-name` is the option used to specify that you want to search by name.
    
-   `[filename]` is the name of the file you're searching for. You can also use wildcards (`*`) in the filename to match multiple files. For example, if you want to search for all text files, you can use `*.txt`.
- 