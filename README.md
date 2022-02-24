# proj4-xv6-rust

### 项目描述
操作系统(OS)内容广泛，单是了解和熟悉相关的概念已足以学习一段时间，比如本科生的一学期课程，而对于 OS 设计与实现的一些细节不容易形成自己的思考。而对于希望对OS有更深入学习和理解的同学，继续了解更多相关的高级主题可能得不偿失。本项目旨在使学生能在设计与实现OS时形成自己的思考，同时更好地掌握OS的基础概念，为之后更高级的主题打下基础。

本项目以`xv6`/`xv6-riscv`为基础，拟采用Rust语言重新设计与实现它。`xv6`/`xv6-riscv` 是MIT-PDOS 实验室以 Unix Version 6 为原型设计并实现的一款面向教学的操作系统, 其配套的课程是 6.S081/6.828。Rust语言与C语言不同，其作为一门现代的系统编程语言，表达能力更强，语义更丰富，所以在用Rust语言参与本项目时，从某种角度上需要我们将一些规则和设计显式地"写"在代码中，这同时也促使了我们去思考。

当前项目实现源码等：

- [https://github.com/Jaic1/xv6-riscv-rust](https://github.com/Jaic1/xv6-riscv-rust)
- [https://github.com/Ko-oK-OS/xv6-rust](https://github.com/Ko-oK-OS/xv6-rust)

### 所属赛道
2022全国大学生操作系统比赛的“OS功能挑战”赛道

### 参赛要求
- 以小组为单位参赛，最多三人一个小组，且小组成员是来自同一所高校的本科生（2022年春季学期或之后本科毕业的大一~大四的学生）
- 如学生参加了多个项目，参赛学生选择一个自己参加的项目参与评奖
- 请遵循“20212国大学生操作系统比赛”的章程和技术方案要求

### 项目导师

齐呈祥 
- github:  https://github.com/KuangjuX
- email: qcx@tju.edu.cn

陈恒杰
- github: [https://github.com/jaic1](https://github.com/Jaic1)
- email: 506933131@qq.com

### 难度

简单~中等

### 特征
- 系统调用接口支持 POSIX 子集，具体可参考[P11 of xv6 book](https://pdos.csail.mit.edu/6.828/2020/xv6/book-riscv-rev1.pdf)
- 使用 Rust 语言实现
- 至少支持 RISCV 平台
- 支持 QEMU 仿真和 Kendryte K210（含MMU和S模式）

### 参考实现
- [xv6-riscv-rust](https://github.com/Jaic1/xv6-riscv-rust)
- [xv6-rust](https://github.com/Ko-oK-OS/xv6-rust)

### License
- MIT license (LICENSE-MIT or [http://opensource.org/licenses/MIT](http://opensource.org/licenses/MIT) )

## 预期目标

### 注意：下面的内容是建议内容，不要求必须全部完成。选择本项目的同学也可与导师联系，提出自己的新想法，如导师认可，可加入预期目标

**注：为了避免重复造轮子，本项目既可以从头开发，也可以联系导师在其项目基础上进行进一步的开发**

### 第一题：从零开始
- 参考本项目也用Rust语言复现 xv6-riscv 的设计与实现

### 第二题：实现和扩展智能指针
- 比如 Arc 和 Condvar 

### 第三题：实现伙伴分配系统
- 实现 Buddy System Allocator 来管理内存

### 第四题：优化进程/线程的调度

- 实现线程机制
- 实现 CFS 或者其他优先级调度算法

### 第五题：支持网络

- 在 QEMU 或者开发板上实现简单的网络驱动和网络协议栈(可以参考一些现有的开源项目，例如 smol-tcp)
- 能够支持 socket 编程
- 能够运行简单的服务器

### 第六题： 移植 SBI 到项目中

- 移植 RustSBI/OpenSBI 到项目中

### 第七题：移植xv6-riscv的实验
- 移植`xv6-riscv`的 [十几个实验](https://pdos.csail.mit.edu/6.S081/2021/labs/)

### 第八题：移植到 RISC-V 开发板上
- Kendryte K210 开发板
- D1 哪吒开发板
- SIFIVE U540, U740 开发板
- 支持在 K210 硬件上运行
