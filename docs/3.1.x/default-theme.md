---
id: default-theme
title: Default Theme
---

import { ColorsBlock, FontBlocks, SpaceBlocks } from "../../src/components/index";

The theme object is where you define your application's color palette, type scale, font stacks, breakpoints, border radius values, and more.

Theming in NativeBase is based on the **[Styled System Theme Specification](https://system-ui.com/theme/)**

## Colors

You can add a `theme.colors` object to provide colors for your project. By default these colors can be referenced by the `color`, `borderColor`, `backgroundColor`, etc.. props.

We recommend adding a palette that ranges from `50` to `900`. Tools like **[Smart Swatch](https://smart-swatch.netlify.app/)**, **[Palx](https://palx.jxnblk.com/)** are available to generate these palettes.

<ColorsBlock/>

## Typography

To manage Typography options, the theme object supports the following keys:

- `fonts` (font families)
- `fontSizes`
- `fontWeights`
- `lineHeights`
- `letterSpacings`

```jsx
const typography = {
  letterSpacings: {
    '2xs': -1.5,
    xs: -0.5,
    sm: 0,
    md: 0.1,
    lg: 0.15,
    xl: 0.25,
    '2xl': 0.4,
    '3xl': 0.5,
    '4xl': 1.25,
    '5xl': 1.5,
  },
  lineHeights: {
    '2xs': 16,
    xs: 18,
    sm: 20,
    md: 22,
    lg: 24,
    xl: 28,
    '2xl': 32,
    '3xl': 40,
    '4xl': 48,
    '5xl': 64,
  },
  fontWeights: {
    hairline: 100,
    thin: 200,
    light: 300,
    normal: 400,
    medium: 500,
    semibold: 600,
    bold: 700,
    extrabold: 800,
    black: 900,
    extrablack: 950,
  },
  fonts: {
    heading: undefined,
    body: undefined,
    mono: undefined,
  },
  fontSizes: {
    '2xs': 10,
    xs: 12,
    sm: 14,
    md: 16,
    lg: 18,
    xl: 20,
    '2xl': 24,
    '3xl': 30,
    '4xl': 36,
    '5xl': 48,
    '6xl': 60,
    '7xl': 72,
    '8xl': 96,
    '9xl': 128,
  },
};
```

<FontBlocks/>

## Size

The `size` key allows you to customize the global spacing and sizing scale for your project. By default these spacing value can be referenced by the `padding`, `margin`, and `top`, `left`, `right`, `bottom` props.

<SpaceBlocks/>

## Opacity

The `opacity` key is mainly used to allow you to define colors opacity using the red-green-blue-alpha (RGBA) model. RGBA color values are an extension of RGB color values with an alpha channel - which specifies the opacity of the color.

```jsx
const opacity = {
  0: 0,
  5: 0.05,
  10: 0.1,
  20: 0.2,
  25: 0.25,
  30: 0.3,
  40: 0.4,
  50: 0.5,
  60: 0.6,
  70: 0.7,
  75: 0.75,
  80: 0.8,
  90: 0.9,
  95: 0.95,
  100: 1,
};
```

## Shadows

The `shadow` key allows you to customize the global box shadow for your project.

```jsx
export default {
  0: {
    shadowColor: '#000',
    shadowOffset: {
      width: 0,
      height: 1,
    },
    shadowOpacity: 0.18,
    shadowRadius: 1.0,
    elevation: 1,
  },
  1: {
    shadowColor: '#000',
    shadowOffset: {
      width: 0,
      height: 1,
    },
    shadowOpacity: 0.2,
    shadowRadius: 1.41,
    elevation: 2,
  },
  2: {
    shadowColor: '#000',
    shadowOffset: {
      width: 0,
      height: 1,
    },
    shadowOpacity: 0.22,
    shadowRadius: 2.22,
    elevation: 3,
  },
  3: {
    shadowColor: '#000',
    shadowOffset: {
      width: 0,
      height: 2,
    },
    shadowOpacity: 0.23,
    shadowRadius: 2.62,
    elevation: 4,
  },
  4: {
    shadowColor: '#000',
    shadowOffset: {
      width: 0,
      height: 2,
    },
    shadowOpacity: 0.25,
    shadowRadius: 3.84,
    elevation: 5,
  },
  5: {
    shadowColor: '#000',
    shadowOffset: {
      width: 0,
      height: 3,
    },
    shadowOpacity: 0.27,
    shadowRadius: 4.65,
    elevation: 6,
  },
  6: {
    shadowColor: '#000',
    shadowOffset: {
      width: 0,
      height: 3,
    },
    shadowOpacity: 0.29,
    shadowRadius: 4.65,
    elevation: 7,
  },
  7: {
    shadowColor: '#000',
    shadowOffset: {
      width: 0,
      height: 4,
    },
    shadowOpacity: 0.3,
    shadowRadius: 4.65,
    elevation: 8,
  },
  8: {
    shadowColor: '#000',
    shadowOffset: {
      width: 0,
      height: 4,
    },
    shadowOpacity: 0.32,
    shadowRadius: 5.46,
    elevation: 9,
  },
  9: {
    shadowColor: '#000',
    shadowOffset: {
      width: 0,
      height: 5,
    },
    shadowOpacity: 0.34,
    shadowRadius: 6.27,
    elevation: 10,
  },
};
```

Still confused? You can always explore [here](https://github.com/GeekyAnts/NativeBase/tree/master/src/theme/base).
