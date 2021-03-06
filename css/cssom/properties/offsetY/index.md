---
title: 'offsetY'
attributions:
  - 'Microsoft Developer Network: [[Windows Internet Explorer API reference](http://msdn.microsoft.com/en-us/library/ie/hh828809%28v=vs.85%29.aspx) Article]'
notes:
  - 'some broken links, readable though.'
readiness: 'Ready to Use'
relationships:
  applies_to:
    predicate: 'Property of '
    value: dom/objects/MouseEvent
    href: '/w/index.php?title=dom/objects/MouseEvent&action=edit&redlink=1'
  return:
    predicate: 'Returns an object of type '
    value: Number
    href: '/w/index.php?title=dom/objects/MouseEvent&action=edit&redlink=1'
standardization_status: 'W3C Working Draft'
summary: 'Gets the y-coordinate of the mouse cursor, relative to the target node.'
tags:
  - API_Object_Properties
  - DOM
todo_broken_links:
  note: 'During import MediaWiki could not find the following links, please fix and adjust this list.'
  links:
    - dom/objects/MouseEvent
    - dom/properties/offsetLeft
    - dom/properties/offsetTop
    - dom/properties/offsetParent
    - dom/objects/DragEvent
    - dom/objects/MouseWheelEvent
    - dom/objects/WheelEvent
    - dom/properties/clientY
    - dom/properties/screenY
uri: css/cssom/properties/offsetY

---
## Summary

Gets the y-coordinate of the mouse cursor, relative to the target node.

Property of [dom/objects/MouseEvent](/w/index.php?title=dom/objects/MouseEvent&action=edit&redlink=1)[dom/objects/MouseEvent](/w/index.php?title=dom/objects/MouseEvent&action=edit&redlink=1)

## Syntax

**Note**: This property is read-only.

``` js
var yCoordinate = event.offsetY;
```

## Return Value

Returns an object of type NumberNumber

The Y coordinate of the mouse cursor.

## Examples

This example uses the **offsetY** property to determine the mouse position relative to the container that fired the event, and also displays the mouse coordinates in the console.

``` html
<!doctype html>
<html>
 <head>
  <style>
#div {
  position:absolute;
  top:200px;
  left:300px;
}
  </style>
  <script>
function offsetCoords(e) {
  var offsetInfo = ""
  offsetInfo = "The x coordinate is: " + e.offsetX + "\n"
  offsetInfo += "The y coordinate is: " + e.offsetY + "\r"
  console.log(offsetInfo);
}
function logCoords(e) {
  console.log("X = " + e.offsetX + " Y = " + e.offsetY);
}
function initialize() {
  document.body.addEventListener("mousemove", logCoords, false);
  document.body.addEventListener("click", offsetCoords, false);
  document.getElementById("div").addEventListener("click", offsetCoords, false);
}
window.addEventListener("load", initialize, false);
  </script>
 </head>
 <body>
  <div id="div">
  </div>
 </body>
</html>
```

## Notes

Offset coordinates include the padding of an element, but not its margin or border.

**TODO**: Check that this is correct.

The coordinates match the [**offsetLeft**](/w/index.php?title=dom/properties/offsetLeft&action=edit&redlink=1) and [**offsetTop**](/w/index.php?title=dom/properties/offsetTop&action=edit&redlink=1) properties of the object. Use [**offsetParent**](/w/index.php?title=dom/properties/offsetParent&action=edit&redlink=1) to find the container object that defines this coordinate system.

## Related specifications

[CSSOM View](http://www.w3.org/TR/cssom-view/)
:   Working Draft

## See also

### Related articles

#### CSSOM

-   [href](/css/cssom/CSSImportRule/href)

-   [media](/css/cssom/CSSImportRule/media)

-   [CSSKeyframeRule](/css/cssom/CSSKeyframeRule)

-   [keyText](/css/cssom/CSSKeyframeRule/keyText)

-   [style](/css/cssom/CSSKeyframeRule/style)

-   [CSSKeyframesRule](/css/cssom/CSSKeyframesRule)

-   [cssRules](/css/cssom/CSSKeyframesRule/cssRules)

-   [deleteRule](/css/cssom/CSSKeyframesRule/deleteRule)

-   [findRule](/css/cssom/CSSKeyframesRule/findRule)

-   [insertRule](/css/cssom/CSSKeyframesRule/insertRule)

-   [name](/css/cssom/CSSKeyframesRule/name)

-   [CSSMediaList](/css/cssom/CSSMediaList/CSSMediaList)

-   [appendMedium](/css/cssom/CSSMediaList/appendMedium)

-   [deleteMedium](/css/cssom/CSSMediaList/deleteMedium)

-   [item](/css/cssom/CSSMediaList/item)

-   [mediaText](/css/cssom/CSSMediaList/mediaText)

-   [CSSMediaRule](/css/cssom/CSSMediaRule/CSSMediaRule)

-   [cssRules](/css/cssom/CSSMediaRule/cssRules)

-   [deleteRule](/css/cssom/CSSMediaRule/deleteRule)

-   [insertRule](/css/cssom/CSSMediaRule/insertRule)

-   [media](/css/cssom/CSSMediaRule/media)

-   [CSSNamespaceRule](/css/cssom/CSSNamespaceRule/CSSNamespaceRule)

-   [namespaceURI](/css/cssom/CSSNamespaceRule/namespaceURI)

-   [prefix](/css/cssom/CSSNamespaceRule/prefix)

-   [CSSOM View](/css/cssom/CSSOM_view)

-   [CSSRule](/css/cssom/CSSRule)

-   [cssText](/css/cssom/CSSRule/cssText)

-   [parentStyleSheet](/css/cssom/CSSRule/parentStyleSheet)

-   [type](/css/cssom/CSSRule/type)

-   [getPropertyPriority](/css/cssom/CSSStyleDeclaration/getPropertyPriority)

-   [clipLeft](/css/cssom/properties/clipLeft)

-   [clipRight](/css/cssom/properties/clipRight)

-   [clipTop](/css/cssom/properties/clipTop)

-   [cssFloat](/css/cssom/properties/cssFloat)

-   [fontWeight](/css/cssom/properties/fontWeight)

-   [hasLayout](/css/cssom/properties/hasLayout)

-   [height](/css/cssom/properties/height)

-   [href](/css/cssom/properties/href)

-   [imports](/css/cssom/properties/imports)

-   [innerWidth](/css/cssom/properties/innerWidth)

-   [isAlternate](/css/cssom/properties/isAlternate)

-   [isPrefAlternate](/css/cssom/properties/isPrefAlternate)

-   [item](/css/cssom/properties/item)

-   [length](/css/cssom/properties/length)

-   [media](/css/cssom/properties/media)

-   [offsetX](/css/cssom/properties/offsetX)

-   **offsetY**

-   [outerHeight](/css/cssom/properties/outerHeight)

-   [outerWidth](/css/cssom/properties/outerWidth)

-   [pageX](/css/cssom/properties/pageX)

-   [pageXOffset](/css/cssom/properties/pageXOffset)

-   [pageY](/css/cssom/properties/pageY)

-   [pageYOffset](/css/cssom/properties/pageYOffset)

-   [pixelBottom](/css/cssom/properties/pixelBottom)

-   [deviceXDPI](/css/cssom/screen/deviceXDPI)

-   [deviceYDPI](/css/cssom/screen/deviceYDPI)

-   [fontSmoothingEnabled](/css/cssom/screen/fontSmoothingEnabled)

-   [height](/css/cssom/screen/height)

-   [style](/css/cssom/style)

-   [type](/css/cssom/style/type)

-   [styleSheet](/css/cssom/styleSheet)

-   [addImport](/css/cssom/styleSheet/addImport)

-   [blockDirection](/css/cssom/styleSheet/blockDirection)

-   [cssRules](/css/cssom/styleSheet/cssRules)

-   [cssText](/css/cssom/styleSheet/cssText)

-   [ownerNode](/css/cssom/styleSheet/ownerNode)

-   [removeImport](/css/cssom/stylesheet/removeImport)

-   [removeRule](/css/cssom/stylesheet/removeRule)

-   [matchMedium](/css/media_queries/apis/matchMedium)

-   [getComputedStyle](/dom/Window/getComputedStyle)

-   [innerHeight](/dom/Window/innerHeight)

-   [styleMedia](/dom/Window/styleMedia)

### Related pages

-   DragEvent[DragEvent](/w/index.php?title=dom/objects/DragEvent&action=edit&redlink=1)
-   MouseEvent[MouseEvent](/w/index.php?title=dom/objects/MouseEvent&action=edit&redlink=1)
-   MouseWheelEvent[MouseWheelEvent](/w/index.php?title=dom/objects/MouseWheelEvent&action=edit&redlink=1)
-   WheelEvent[WheelEvent](/w/index.php?title=dom/objects/WheelEvent&action=edit&redlink=1)
-   `Reference`
-   clientY[clientY](/w/index.php?title=dom/properties/clientY&action=edit&redlink=1)
-   pageY[pageY](/css/cssom/properties/pageY)
-   screenY[screenY](/w/index.php?title=dom/properties/screenY&action=edit&redlink=1)
-   y[y](/css/cssom/properties/y)
