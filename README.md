# 交互式 3D 掷骰子器【中文翻译版本】
##### 来源于 [a.teal.info/dice](https://a.teal.info/dice)

一款在线交互式 3D 掷骰子器，使用了 `three.js` 和 `cannon.js`。它使用 [random.org](https://random.org) 提供的 API，为 d4、d6、d8、d10、d12、d20 和 d100 的任意组合生成真正的随机掷骰子。屏幕上显示的物理值仅用于展示，所有数值均来自大气噪声。

### 使用方式

#### URL 参数

有几个参数可以传入 URL。使用参数的语法是： `matteas.nz/dice-roller?<param>[=<value>]`

##### 颜色
通过在 URL 中添加 `color=<color>`，可以更改骰子的颜色。如果没有指定此参数，默认颜色为黑色。目前支持的颜色有：

- White (#808080)
- Blue (#1883db)
- Red (#d10e00)
- Green (#008a17)
- Orange (#fc7b03)
- Purple (#7d0099)
- Brown (#593304)

##### 符号

By adding `notation=<notation>` to the URL, you can set the dice roll to be executed. This is useful when you want to know the result of a very specific dice roll without needing to first input that roll on the site. Note that `roll` is still needed to roll the dice without pressing the button on the site. This project uses the standard dice notation which you can read more about [here](https://en.wikipedia.org/wiki/Dice_notation). Some examples:

| Notation | Result |
| -------- | ------ |
| 1d6      | A single 6-sided die |
| 2d10     | Two 10-sided die |
| 1d8 + 1d20 | A single 8-sided die and a single 20-sided die |

##### Roll

By adding `roll` to the URL, you can intiate a rolling of dice directly without
the need to press the button on the site. There is no value associated with
this parameter, so the usage is simply `matteas.nz/dice-roller?roll`.

##### Shadows

禁用掷出骰子的阴影渲染， 在 URL 中添加 `shadows=0`。请注意，这不会影响选择屏幕上的阴影，只会影响掷骰子时的阴影。

### Demo

在线演示: https://dice-roller.game.996.ninja

![](dice-roller-demo.gif)

### License

*Interactive 3D Dice Roller* is licensed under the MIT License.

### 版权

原始代码的所有权利属于 [Anton Naratov](http://www.teall.info/)。本项目只是建立在他的工作基础之上。
