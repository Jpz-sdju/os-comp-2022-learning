# day02

### 今日已完成的计划

1.在工位电脑上安装虚拟环境

2.学习RUST圣经1.1-1.6，了解cargo和dependency等概念。

3.学习RUST圣经2.1

4.学习RUST圣经2.2.1

5.学习RUST圣经2.2.2

### 完成过程

1.碰到一个小小的坑，rustup的doc若使用firefox默认打开的话好像会失败，安装了稳定版的chrome就可以了。

由于oslab虚拟机自带vscode和rust的runtime，所以也算偷了个小懒。不过以前安装过很多次虚拟机，可以保证以后不会由于偷懒掉进坑里（也许）。

---

2.使用cargo run和build了一点代码，看了看toml和lock文件的区别。把crate.io的镜像改成了ustc的。

---

3.了解了let和mut的区别，虽然个人之前对于声明可变变量和声明不可变变量的区别没有可以关注过（也没有接触过类似语言，除了scala & chisel），感觉日后可能会在这个方面踩坑。

---

4.float类型无法作为hashmap的key，因为没有实现std::cmp::eq特征！并且在浮点数进行操作（尤其是大于小于等于这种运算)时要非常小心！

可以在等号右边值后写类型;=>

let x = 8i32;

let y = 4.5f32;

let y = 4.6_f32;

可以使用{:.xxx}省略小数点，其他格式和C差不多，只不过在冒号：后而已。

---

5.记录重要点： ''只能留给字符，“”只能留给字符串。
