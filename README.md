# capslox-karabiner

本项目是基于karabiner实现替代[capslox软件](https://capslox.com)
部分功能的配置，由于在内测阶段一直使用capslox，且仅使用了基础热键，故没有参与付费购买，当然capslox不得不说是一款在Mac上非常好用的软件。

## 安装

1. 下载 [Karabiner-Elements](https://karabiner-elements.pqrs.org/) 并安装好
2. 在默认浏览中输入下面网址，并回车
    ```shell
    karabiner://karabiner/assets/complex_modifications/import?url=https://raw.githubusercontent.com/zhechen/capslox-karabiner/main/capslox-karabiner.json
    ```
3. 跳转至Karabiner-Elements并导入
4. 在软件菜单项 `Complex modifications` 中点击左下角 `Add rule` 启用该项目全部功能

![img](https://pic.yqqy.top/blog/202112231454280.jpg?imageMogr2 "效果图1")

**注意：**

如果要外接键盘，需要将command键位与option键位互换，如下：

![img](https://pic.yqqy.top/blog/202112231505410.jpg "效果图2")

## 认识键盘符号

README下文将用以下符号来表示按键位及映射键位，其代表释义如下：

| 符号 | Name     | 符号    | Name      |
| ---- | -------- | ------- | --------- |
| `⇪`  | Capslock | `↖`     | Home      |
| `⎋`  | Escape   | `↘`     | End       |
| `⌘`  | Command  | `⇞`     | Page Up   |
| `⌥`  | Option   | `⇟`     | Page Down |
| `⌃`  | Control  | `🖱️` `L` | 鼠标左击  |
| `⇧`  | Shift    | `🖱️` `R` | 鼠标右击  |
| `⌫`  | Delete   | `🖱️` `F` | 鼠标前进  |
|      |          | `🖱️` `B` | 鼠标后退  |

## 用法

### Capslock赋能

将Capslock赋能为一个全新的功能修饰键 **✱ Hyper** ，类似于同时按下 `⇧` `⌃` `⌥` `⌘`

| 按键     | 映射为       | 说明                  |
| -------- | ------------ | --------------------- |
| `⇪ 点击` | `⎋` Escape   | 单击Capslock发送ESC   |
| `⇪ 按住` | `✱` Hyper    | 按住Capslock启用Hyper |
| `✱` `⎋`  | `⇪` Capslock | 单击ESC切换大写锁定   |
| `✱` `␣`  | `⌃` `␣`      | 单击空格切换输入法    |

### 光标移动

长按 **Capslock (✱ Hyper) 键** 配合进行操作

| 按键    | 映射为     | 说明       |
| ------- |---------|----------|
| `⇪` `E` | `↑`     | 向上移动     |
| `⇪` `D`     | `↓`     | 向下移动     |
| `⇪` `S`     | `←`     | 向左移动     |
| `⇪` `F`     | `→`     | 向右移动     |
| `⇪` `A`     | `⌥` `←` | 向左移动一个单词 |
| `⇪` `G`     | `⌥` `→` | 向右移动一个单词 |
| `⇪` `P`     | `⌘` `←` | 移动至行首    |
| `⇪` `;`     | `⌘` `→` | 移动至行尾   |
| `⇪` `⌥` `P` | `⌃` `A` | 移动至行首增强  |
| `⇪` `⌥` `;` | `⌃` `E` | 移动至行尾增强 |
| `⇪` `⌘` `P` | `⇞`     | 移动至页首  |
| `⇪` `⌘` `;` | `⇟`     | 移动至页尾    |

### 光标选中

| 按键 | 映射为 | 说明       |
| ---- | ------ |----------|
| `⇪` `I`  | `⇧` `↑` | 向上选中     |
| `⇪` `K`  | `⇧` `↓` | 向下选中     |
| `⇪` `J`  | `⇧` `←` | 向左选中     |
| `⇪` `L`  | `⇧` `→` | 向右选中     |
| `⇪` `H`  | `⇧` `⌥` `←` | 向左选中一个单词 |
| `⇪` `N`  | `⇧` `⌥` `→` | 向右选中一个单词 |
| `⇪` `Y`     | `⌥` `↑` | 向外括选区域   |
| `⇪` `B`     | `⌥` `下` | 向内缩减区域   |
| `⇪` `U`  | `↖` `←` | 选中至行首    |
| `⇪` `O`  | `↘` `→` | 选中至行尾    |
| `⇪` `⌘` `U` | `⌥` `⇞` | 选中至页首    |
| `⇪` `⌘` `O` | `⌥` `⇟` | 选中至页尾    |
| `⇪` `,` | `⌥` `←`  +  `⇧` `⌥` `→` | 选中当前单词   |
| `⇪` `⌘` `,` | `↖`  +  `↘` `→` | 选中当前行 |
| `⇪` `⌘` `I` | `⇧` `⌥` `↑` | 选中的行向上移动 |
| `⇪` `⌘` `K` | `⇧` `⌥` `↓` | 选中的行向下移动 |

### 文本删除

| 按键         | 映射为   | 说明     |
| ----------- | -------- | -------- |
| `⇪` `W`     | `⌫`      | 向左删除 |
| `⇪` `R`     | `fn` `⌫` | 向右删除 |
| `⌘` `⇪` `W` | `⌥` `⌫` | 向左删除一个单词 |
| `⌘` `⇪` `R` | `⌥` `fn` `⌫` | 向右删除一个单词 |
| `⇪` `[` | `↖` `←`  +  `⌫` | 删除至行首 |
| `⇪` `/` | `↘` `→`  +  `⌫` | 删除至行尾 |
| `⇪` `⌫` | `⌘` `⌫` | 删除当前行 |
| `⇪` `⌘` `⌫` | `⌘` `A`  +  `⌫` | 删除全部内容 |

### 鼠标操作

| 按键        | 映射为  | 说明     |
| ----------- | ------- | -------- |
| `⇪` `🖱️` `L` | `🖱️` `F` | 鼠标前进 |
| `⇪` `🖱️` `R` | `🖱️` `B` | 鼠标后退 |

## 参考项目

- [https://github.com/BryanHoo/Capslock-Plus](https://github.com/BryanHoo/Capslock-Plus)
- [https://github.com/Vonng/Capslock](https://github.com/Vonng/Capslock)
