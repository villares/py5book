# Py5MouseEvent.is_alt_down()

Return boolean value reflecting if the Alt key is down.

## Examples

<div class="example-table">

<div class="example-row"><div class="example-cell-image">

</div><div class="example-cell-code">

```python
def setup():
    py5.size(200, 200)
    py5.rect_mode(py5.CENTER)


def draw():
    py5.square(py5.random(py5.width), py5.random(py5.height), 10)


def mouse_clicked(e):
    if e.is_alt_down():
        py5.println('the alt key is down')
    else:
        py5.println('the alt key is not down')
```

</div></div>

</div>

## Description

Return boolean value reflecting if the Alt key is down. The Alt key is a modifier key and can be pressed at the same time as other keys.

Underlying Processing method: isAltDown

## Signatures

```python
is_alt_down() -> bool
```

Updated on March 06, 2023 02:49:26am UTC
