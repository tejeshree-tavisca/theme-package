# **ORXe Theme**

This ORXe base theme package contains the predefined base theme colors, mixins and functions useful for the ORXe components.

## **Installation**

```bash
npm install @orxe/theme
```

---

## **Import**

To use the orxe base theme, simply use the following **`import`** statement in your component's map **`scss`** file.

*Specify the name of your component in place of `<component-name>` below*

```css
@import "@orxe/theme/components/<component-name>/variables.scss";
```
---

## **Usage**

#### **Using theme colors**

```css
/* Set styling for a checkbox element */
/* _component.scss */
.checkbox {
  &::before {
    background-color: $checkbox-background-color;
    border: $checkbox-border-width solid $checkbox-border-color;
  }

  &.selected {
    &::before {
      background-color: $checkbox-background-color-selected;
      border: $checkbox-border-width solid $checkbox-border-color-selected;
    }
  }

  &.disabled {
    &::before {
      background-color: $checkbox-background-color-disabled;
      border: $checkbox-border-width solid $checkbox-border-color-disabled;
    }
  }
}
```

#### **Using mixins & functions**

```css
/* _component.scss */
button {
  @include border-radius(5px); // mixin to apply border-radius to all sides
  height: calculate_rem(24px); // function to convert px to rem
  width: 100%;
}
```

---

## **Global Colors**

| Color Variable  | Color Code (HEX) |
| --------------- | ---------------- |
| \$primary       | #238738          |
| \$secondary     | #0A57A1          |
| \$tertiary      | #13294E          |
| \$error         | #D9222A          |
| \$separator-01  | #E1E6ED          |
| \$background-01 | #F5F8FB          |
| \$neutral       | #FFFFFF          |

---

## **Text Colors**

| Color Variable   | Color Code (HEX) |
| ---------------- | ---------------- |
| \$primary-text   | #242C38          |
| \$secondary-text | #505660          |
| \$tertiary-text  | #6A7078          |
| \$disabled       | #969DA4          |
| \$links          | #0A57A1          |
| \$pricing        | #238738          |
| \$error          | #D9222A          |
| \$neutral        | #FFFFFF          |

---

## **Mixins**

| Mixin Name         | Uses                                                                                                             |
| ------------------ | ---------------------------------------------------------------------------------------------------------------- |
| border-radius      | To apply border radius to all sides of an element                                                                |
| padding            | To apply padding to all side of an element                                                                       |
| padding-horizontal | To apply padding to left & right sides only of an element                                                        |
| margin             | To apply margin to all side of an element                                                                        |
| margin-horizontal  | To apply margin to left & right sides only of an element                                                         |
| font-smoothing     | For font smoothing                                                                                               |
| text-inherit       | To inherit all properties of a parent element<br>font-family, font-size, font-style, font-weight, letter-spacing |

---

## **Functions**

| Function Name | Uses                                                      |
| ------------- | --------------------------------------------------------- |
| calculate_em  | To convert px into em                                     |
| calculate_rem | To convert px into rem                                    |
| encode-svg    | To encode svg for background images                       |
| str-replace   | It is useful to provide dynamic string                    |

---
