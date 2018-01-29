---
layout: post
title: Font Ligatures Are Awesome
description: "Using fonts that have ligatures helps my code look more readable and - more importantly - cool 😎"
date: 2018-01-29
tags: [font, design, code, style]
comments: false
share: false
---

If you're like me, a Hipster Coder™, you probably love perfectly tweaking your color themes and fonts on a regular basis to try to find that perfect combination.

Recently, I've been learning about a new way to up your coding font game - font **ligatures**.

> In writing and typography, a ligature occurs where two or more graphemes or letters are joined as a single glyph.

A ligature for electronic fonts is basically a symbol that is used to represent two separate typed characters in a given combination.  It joins two characters into one to better represent it on the screen.

## Fira Code

An awesome monospace font that I've been using is Fira Mono, characterized by it's cool and serif-like lowercase 'r' character and angular 'j'.  I recently ran across an open source extension of the Fira Mono font that include these awesome ligatures called [Fira Code](https://github.com/tonsky/FiraCode).

Fira Code takes an already solid monospace font, and introduces a ton of useful ligatures for coding.  Including ligatures for comparison operators, comments and arrows, and arithametic operators.

![fira code mono comparison](https://github.com/tonsky/FiraCode/blob/master/showcases/all_ligatures.png?raw=true)

## Using Fira Code

I used the [instructions](https://github.com/tonsky/FiraCode/wiki) from the Fira Code GitHub to install the font.

Fira Code is compatible with a bunch of [different editors](https://github.com/tonsky/FiraCode#editor-support) as well as terminal support.  I'm currently using it in Terminal on mac as well as Atom and Android Studio.

## My Fira Code Configurations

### Android Studio

In Android Studio under `Settings` → `Editor` → `Colors & Fonts` → `Font`

![android studio font preferences](https://github.com/robotsquidward/robotsquidward.github.io/blob/master/images/android-font-preferences.png?raw=true)

*Also check out [Hack](https://github.com/source-foundry/Hack) - another great coding font I have used.*

### Atom

In Atom I wanted not only Fira Code, but to try to use Fira Code with an additional italic font to mimic '[Operator](https://www.typography.com/blog/introducing-operator)', a fancy (expensive) monospaced font with many similarities to Fira Code.

In Atom, you can set the font easily in `Settings` → `Editor`

![atom editor preferences](https://github.com/robotsquidward/robotsquidward.github.io/blob/master/images/atom-preferences-1.png?raw=true)

To enable font ligatures for Fira Code, include this snippet in your Atom `styles.less`

```css
atom-text-editor {
  text-rendering: optimizeLegibility;

  &.editor .syntax--string.syntax--quoted,
  &.editor .syntax--string.syntax--regexp {
    -webkit-font-feature-settings: "liga" off, "calt" off;
  }
}
```

In addition, if you download and install [Script12 BT](https://www.myfontsfree.com/134618/script12pitchbt.htm), an italic cursive-styled mono font, you can add this snippet to make key words use that font for an Operator feel.

```css
atom-text-editor.editor {
  /*
    Transform selected text into alternative font for elegant touch:
    - this
    - HTML and JSX attributes
    - JS functions (except arrow function)
    - JS undefined
    - JS storage (const/let/async)
    - EX constants
    - Ruby (nil/self/block)
    - Ruby hash keys
  */
  .syntax--variable.syntax--language.syntax--this,
  .syntax--html > .syntax--attribute-name,
  .syntax--JSXAttrs > .syntax--attribute-name,
  .syntax--storage.syntax--type.syntax--js:not(.syntax--function):not(.syntax--arrow),
  .syntax--constant.syntax--language.syntax--undefined.syntax--js,
  .syntax--constant.syntax--other.syntax--object.syntax--key.syntax--js,
  .syntax--variable.syntax--other.syntax--constant.syntax--elixir,
  .syntax--constant.syntax--language.syntax--elixir,
  .syntax--constant.syntax--language.syntax--nil.syntax--ruby,
  .syntax--variable.syntax--language.syntax--self.syntax--ruby,
  .syntax--constant.syntax--other.syntax--symbol.syntax--hashkey.syntax--ruby,
  .syntax--variable.syntax--other.syntax--block.syntax--ruby {
    vertical-align: baseline;
    font-size: 100%;
    font-style: italic !important;
    height: inherit;
    line-height: 100%;
  }
}
```

The result, something like this:

![atom preview](https://github.com/klippx/operator-mono-atom/blob/master/img/JSX.png?raw=true)

Check out [operator-mono-atom](https://github.com/klippx/operator-mono-atom) to learn more.

### Mac Terminal

Terminal nicely supports ligatures out of the box, just use Fira Code as your font!

![terminal preferences](https://github.com/robotsquidward/robotsquidward.github.io/blob/master/images/terminal-preferences.png?raw=true)

## Other Fonts

If you don't love Fira Code, but you love the idea of ligatures in your code, there are plenty of other fonts that support ligatures that you can check out.

- [Hasklig](https://github.com/i-tu/Hasklig) (free)
- [PragmataPro](http://www.fsd.it/fonts/pragmatapro.htm)
- [Monoid](http://larsenwork.com/monoid/) (free)
- [Fixedsys Excelsior](https://github.com/kika/fixedsys) (free)
- [Iosevka](https://be5invis.github.io/Iosevka/) (free)
- [DejaVu Sans Code](https://github.com/SSNikolaevich/DejaVuSansCode) (free)

## Fonts are fun

Hope you had a good time if you were looking to amp up your coding editor font!  Tell your friends more about ligatures and watch them be wowed by your vocabulary and typographic knowledge.

Please let me know [@ajkuterman](http://twitter.com/ajkueterman) if you have any other fonts or IDE configurations you want to tell me more about!  Always looking to make things pretty when I code.
