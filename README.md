# Media Query Breakpoints
Using mixin and variables to simplify Sass media query / breakpoints.

## Usage
```css
@import 'mixins';
@import 'variables';

.sample {
    display: grid;
    grid-template-columns: 330px;
    grid-template-rows: 1fr;

    @include breakpoint($tablets) {
        grid-template-columns: repeat(2, 330px);
    }

    @include breakpoint($laptops) {
        grid-template-columns: repeat(3, 330px);
    }

    @include breakpoint($desktops) {
        grid-template-columns: repeat(4, 330px);
    }    
}
```
