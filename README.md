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

### Classes

To apply style from **Quill**, you must use classes on element to customize them.

#### Background

The class `background` can be used to apply a background color and matching font color on a element. In combination with `background`, both `light` and `dark` allow to choose the background darkness.
The special case of `above` allow to set a hightlighted background depending on the background below.

#### Layout

Both classes `row` and `column` alow to create a flex container in the given direction.
The distribution of the children can be defined by the classes `from-start` for start of the container, `from-end` for end of the container, `gapped` for space between children, `spaced` for space around children.
The alignement of the children can be defined by the classes `at-start` for start of the container, `at-end` for end of the container and `at-center` for center of the container.
The class `stretch` allow the children to take full place in the cross axis. In a column, it will result with children of column full width. In a row, children will be full height.

#### Spacing

Both classes `margin` and `padding` to set the matching spacing.
The classes `step`, `near`, `midrange` and `far` can be used to define the space size.
The classe prefixes `horizontal-`, `vertical-`, `top-`, `right-`, `bottom-`, `left-` can be used with either `margin` or `padding` to specify the direction of the space.
