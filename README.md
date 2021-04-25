# Draggable

This JS library lets you make adding drag and drop to your HTML dead simple.
E.g.,

```html
<!-- Draggable container -->
<div data-draggable>
    <!-- data-highlight-draggable tells a whole area that it can be dropped to -->
    <!-- The ids will be swapped -->
    <div id=_1 data-highlight-draggable>
        <!-- Tells that this element actually allows it to be dragged -->
        <div draggable=true>
        </div>
    </div>
    <div id=_2 data-highlight-draggable>
        <!-- Tells that this element actually allows it to be dragged -->
        <div draggable=true>
        </div>
    </div>
</div>
```

Once the swap happens a custom event called `swapped` will be dispatched at the
`document` level with `detail` object with properties `source` and `target` will
be sent.

