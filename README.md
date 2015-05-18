# rowlow.utils.colors

Defining a map of color name and color code pairs, this module generates css selectors for each background, border and text colors.

## Install

```
    bower install --save rowlow.utils.colors
```

## Variables

```
    $rowlow-colors-namespace // Specific module namespace
    $rowlow-colors // Map of colors
```

## Functions
```
    $rowlow-color()
```

## Usage

### Setup
```
    /* Set modules namespace (optional) */
    $rowlow-colors-namespace: "namespace-";

    /* Define color map */
    $rowlow-colors: (
        "white":    #ffffff,
        "black":    #000000,
        "grey":     #cccccc
    );

    @import "bower_components/rowlow.utils.colors/main.scss"
```

### SCSS
```
    /* Get color code using a function */
    body{
        background-color: rowlow-color("grey");
    }
```

### HTML
```
    <!-- Setting a background color via selector -->
    <body class="background-color--grey"></body>

    <!-- Setting a text color via selector -->
    <h1 class="text-color--grey"></h1>

    <!-- Setting a border color via selector -->
    <h1 class="border-color--grey"></h1>
```
