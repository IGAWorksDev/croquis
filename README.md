# croquis
the lightweight rendering library of Homeworks

## what is croquis

croquis is the rendering library built-in to Homeworks

truth of typing and light weight size of library is the key of the purpose

it will be monkey patched in homeworks however you can use it by directly importing (global context)

croquis has the advantage of having state on MVW base unlike other libraries

croquis follows virtuam dom structure, state strategy. it is so fast :zap:!

## what is difference between jquery?

jquery is an intuitive rendering library, however it has some risks

dynamic types could be occured unexpected error

and event binding will be deleted when the element is removed

and also DOM access is slow without convention

in other words, the optimization makes the running curve steep

## design

```javascript
Method('component', {
    init: function() {
        // mongkey-patched context searching
        hand('target')
            // width is a constant
            .css(width, 100)
            .attr(href, '#')
            .attr('customAttr', 'hello')
            .data('key', 'ok')
            .stat(disabled, false)
            .stop()
            .on(click, () => {
                // it is exactly the same as hand.logger.debug()
                hand.logger('clicked!');
            })
            .anim(width, 100)
            .remove()
            // restore will recreate 
            .restore();
    }
});
```
