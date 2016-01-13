# [row] and [col]

The *row* and *col* shortcodes should always be used in conjunction with each other for when you want to lay out your content in multiple columns. One or more *col* sections should be wrapped by a *row* shortcode to encapsulate a single row of columns. For example:

```
[row]

[col sm="6"]
Column one content goes here…
[/col]

[col sm="6"]
Column two content goes here…
[/col]

[/row]
```

While the *row* shortcode can only accept a class attribute to add supplementary CSS classes to the generated HTML, the *col* shortcode can interpret a wide selection of attributes that control that column's appearance:

* **xs, sm, md, lg:** Specifies the number of twelve available columns you wish to span within the row for the four main screen sizes.
* **xs_offset, sm_offset, md_offset, lg_offset:** Increases the left margin of a column by a given number of columns.
* **xs_push, xs_pull, sm_push, sm_pull, md_push, md_pull, lg_push, lg_pull:** Used to change the visual order of the columns by "pushing" or "pulling" by a given number of columns.
* **class:** Any extra CSS classes you wish to add to the column's HTML element.

So, for the example provided above, this combination of row and col shortcodes would generate two even, 50% width columns of content on small screen sizes and up.