# Quill

**Quill** is a very lightweight CSS toolbox for standardized and common style.

## Usage

You can directly include the `styles` folder into a project and link to the main file `styles/Quill.css` or use a CDN that interface Github like jsDelivr : [https://cdn.jsdelivr.net/gh/louis-parent/Quill@main/styles/Quill.css](https://cdn.jsdelivr.net/gh/louis-parent/Quill@main/styles/Quill.css).

## Documentation

### Variables

**Quill** uses CSS variables to automatically generate customized style.

#### Colors

There are three important CSS variables for color to set :

- `--primary` : the primary color is used to make identifiable components
- `--secondary` : the secondary color is used to make accent components
- `--neutral` : the neutral color is used for background and foreground generic colors

There are four semantic color that can be modified for a more fined grained customization :

- `--info-color`
- `--success-color`
- `--warning-color`
- `--error-color`

For each of these color (primary, secondary and semantics) there a variable for the font color over it named `--on-[COLOR]-color`.

#### Fonts

There are three font levels :

- `--headline-font` : Used for title text
- `--paragraph-font` : Used for all the text by default
- `--exotic-font` : Used for special emphasis text

#### Spaces

There are four space range :

- `--step-space` : Used for separator without space
- `--near-space` : Used for smallest space
- `--midrange-space` : Used for medium space
- `--far-space` : Used for biggest space

#### Rounding

There are four rounding radius :

- `--soft-rounded-radius` : Used for discrete radius
- `--rounded-radius` : Used as the standard radius
- `--very-rounded-radius` : Used for oval elements like pills
- `--circular-radius` : Used for circular elements

### Classes

To apply style from **Quill**, you must use classes on element to customize them.

#### Background

The class `background` can be used to apply a background color and matching font color on a element. In combination with `background`, both `light` and `dark` allow to choose the background darkness.
The special case of `above` allow to set a hightlighted background depending on the background below.

#### Layout

Both classes `row` and `column` alow to create a flex container in the given direction.
The distribution of the children can be defined by the classes `from-start` for start of the container, `from-center` for center of the container, `from-end` for end of the container, `gapped` for space between children, `spaced` for space around children.
The alignement of the children can be defined by the classes `at-start` for start of the container, `at-end` for end of the container and `at-center` for center of the container.
The class `stretch` allow the children to take full place in the cross axis. In a column, it will result with children of column full width. In a row, children will be full height.
The class `wrap` allow wrapping for the flex container.
The class `reverse` allow to reverse the whole flex container.

#### Spacing

Both classes `margin` and `padding` to set the matching spacing.
The suffixes `-step`, `-near`, `-midrange` and `-far` can be used to define the space size.
The classe prefixes `horizontal-`, `vertical-`, `top-`, `right-`, `bottom-`, `left-` can be used with either `margin` or `padding` to specify the direction of the space.
The special prefix `no-` can be used before any composed spacing to disable the space in this direction.

#### Sizing

The classes `width` and `height` can be used to defined the size of an element. Four prefixes are available for different sizes : `full-`, `three-quarter-`, `two-third-`, `half-`, `third-` and `quarter-`.
The alternive classes `screen-width` and `screen-height` can be used to base the size relative to viewport.
The suffixes `-max` and `-min` can be used to set maximal and minimal sizing.

#### Positionning

The classes `relative`, `sticky`, `fixed`, `absolute` can be used to set the matching positionning mode. The class `offset` indicate to use `--offset-x` and `--offset-y` CSS variables for relative and sticky position. The class `coordinate` indicates to use `--x` and `--y` CSS variables for fixed and absolute positionnig.
The classes `behind`, `front` and `always-on-top` are used for depth of positionated elements.

#### Rounding

There are four level of rounded border. `soft-rounded` class is used for a discrete rounding, `rounded` class is a standard rounded element, `very-rounded` is class for element like pills, and `circular` make the element circular.

#### CTA

CTA are emphasis interactible elements defined with the class `cta`.
There are variant with both class `primary` and `secondary` to choose the color.
By default the CTA is fully colored, but the class `discrete` only emphasis the border.
The class `floating` make a circular CTA like floating button.
The class `icon-prefixed` is a special class for CTA composed of an icon and a content.

#### Input

Input can be styled in two ways associated with two classes `filled` and `outlined`. Filled input has a neutral background and is underlined, outlined input has no background and a complete border.
Color of the input can be set with with the `primary` and `secondary` classes.

#### Text

Standard text formatting can be easily done with some classes.
The font can be modified with `bold` and `italic`.
The font case can be set with `uppercase`, `lowercase` and `capitalized`.
The font lines can be defined with `underlined`, `overlined` and `crossed-out`. The optional class `solid`, `double`, `dotted`, `dashed` and `wavy` can define the style of the line. The classes `primary`, `secondary`, `neutral`, `info`, `success`, `warning`, `error` can be used to set a custom color for the line.
