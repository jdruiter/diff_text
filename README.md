# diff_text
Computes the difference between two texts and returns output as html (Python)

* Compare two blocks of plain text and efficiently return a list of differences.
* [Diff Demo](https://neil.fraser.name/software/diff_match_patch/demos/diff.html)

Forked and expanded from: 
https://github.com/google/diff-match-patch

# Example 1:

```from diff_text import htmldiff
htmldiff("Hello World.", "Goodbye World.")
```

# Example 2:

```from diff_text import diff_match_patch
dmp = diff_match_patch()
diff = dmp.diff_main("Hello World.", "Goodbye World.")
Result: [(-1, "Hell"), (1, "G"), (0, "o"), (1, "odbye"), (0, " World.")]
dmp.diff_cleanupSemantic(diff)
print(diff)
Result: [(-1, "Hello"), (1, "Goodbye"), (0, " World.")]
```
