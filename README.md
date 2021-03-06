# auto-close-html2 package

There are some auto close html tag packages on atom.io, but they all have sort of bugs and it seems that the owners don't want to maintain the packages anymore. So I copied a package from [autoclose](https://atom.io/packages/autoclose) , and fixed its bug.

![A screenshot of your package](https://raw.githubusercontent.com/yubaoquan/yubaoquan.github.io/master/images/auto-close-html2-demo/demolow.gif)

# Settings
- `Add Slash To Self Close Tag`: Auto add a slash when close a self-close tag.
- `Enabled File Types`: Files with these extensions will trigger auto close, default file type is `html`. (comma split)
- `Insert Whitespace On Close`: Auto add a whitespace if tag is self-close and there is no whitespace before `>` or `/>`
- `Self Close Tags`: Define your own custom self-close tags, these tags will behave like self-close tags like `img`, `br`. (comma split)
- `Slash Trigger Auto Close`: When typing slash and the tag is self-close tag, close the tag.

# Changelog

### 0.2.0
- Fix slash bug of autoclose.

### 0.3.0
- Enable selfclose tags configuration.
- Fix typing > cause auto add right part tag to selfclose tags.

### 0.3.2
- Fix tag attributes take up multi lines cause auto close not work.

### 0.3.3
- Fix bugs produced by 0.3.2

### 0.3.4
- Stop continue close tag logic when typing slash or > in template brackets like`{#if a / b > c}`.

### 0.3.5
- Auto backspace indent for tags that across multiple lines like this:

before 0.3.5
```
<div
    aaa="bbb"
    ></div>
```
after 0.3.5
```
<div
    aaa="bbb"
></div>
```

### 0.3.6
- Add changelog of 0.3.5


### 0.3.8
- Auto close comment tag

![A screenshot of 0.3.7](https://raw.githubusercontent.com/yubaoquan/yubaoquan.github.io/master/images/auto-close-html2-demo/commentDemo.gif)

### 0.4.1
- Add freemarker support

### 0.5.0
- Add 3 more options for self-close tag

### 0.5.1
- Update readme

### 0.6.0
- Change `Disabled File Extensions` to `Enabled File Types` because I think file type having html-like content is less than file type not having html-like content.

- Auto detect and use the editor setting of `Tab Type` and `Tab Length`. If tab type is set to `hard`, the indent in `auto-close-html2` will be tab, otherwise whitespace.

### 0.6.1
- Update description of settings.

### 0.7.0
- Add `@` to tagName regexp
