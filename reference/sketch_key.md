# key

The variable `key` always contains the value of the most recent key on the keyboard that was used (either pressed or released).

## Examples

<div class="example-table">

<div class="example-row"><div class="example-cell-image">

</div><div class="example-cell-code">

```python
# click on the window to give it focus,
# and press the 'b' key.

def draw():
    if py5.is_key_pressed:
        if py5.key in ['b', 'B']:
           py5.fill(0)
    else:
        py5.fill(255)

    py5.rect(25, 25, 50, 50)
```

</div></div>

</div>

## Description

The variable `key` always contains the value of the most recent key on the keyboard that was used (either pressed or released). 
 
For non-ASCII keys, use the [](sketch_key_code) variable. The keys included in the ASCII specification (`BACKSPACE`, `TAB`, `ENTER`, `RETURN`, `ESC`, and `DELETE`) do not require checking to see if the key is coded, and you should simply use the `key` variable instead of [](sketch_key_code). If you're making cross-platform projects, note that the `ENTER` key is commonly used on PCs and Unix and the `RETURN` key is used instead on Macintosh. Check for both `ENTER` and `RETURN` to make sure your program will work for all platforms.

There are issues with how [](sketch_key_code) behaves across different renderers and operating systems. Watch out for unexpected behavior as you switch renderers and operating systems.

Underlying Processing field: [key](https://processing.org/reference/key.html)

Updated on December 07, 2024 22:07:08pm UTC
