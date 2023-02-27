# check if a string contains a specific word or substring in PHP

To check if a string contains a specific word or substring in PHP, you can use the strpos or stripos function.

Here's an example code snippet:

```
$string = "This is a sample string.";
$word = "sample";

if (strpos($string, $word) !== false) {
    echo "The string contains the word '$word'.";
} else {
    echo "The string does not contain the word '$word'.";
}
```
In the above code, strpos function is used to find the position of the first occurrence of $word in $string. If the $word is not found, strpos returns false, so the !== false comparison is used to check if the word exists in the string.

You can use stripos instead of strpos to perform a case-insensitive search.

```
$string = "This is a sample string.";
$word = "SAMPLE";

if (stripos($string, $word) !== false) {
    echo "The string contains the word '$word'.";
} else {
    echo "The string does not contain the word '$word'.";
}
```
