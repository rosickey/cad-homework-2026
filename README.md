# 电子线路 CAD 课程作业提交说明（学生版）

课程仓库：<https://github.com/rosickey/cad-homework-2026>

本课程使用 GitHub Pull Request（PR）提交作业。每位同学固定使用自己的：

- GitHub 账号；
- 9 位学号分支；
- `students/学号/` 目录。

例如，11 专业 1 号学生的学号为 `240201101`，则对应关系必须是：

```text
分支：240201101
目录：students/240201101/
```

> 重要：学生只能修改自己的学号目录。不要修改 `README.md`、`.github/`、`assignments/` 或其他同学的目录。

本文中的 Windows 命令均在 **Git Bash** 中执行。除非教师特别说明，不要把命令直接输入 Windows 的 CMD。

## 第一次提交没有通过的同学，请尽快修改（所有同学先完成第一次提交，作业之后再交）

# CAD 学生注册 PR 错误处理简表

| PR | 学号 | 姓名 | 原因 |
| --- | --- | --- | --- |
| 11 | 240201106 | 曹敏 | 来源分支必须为 9 位学号 |
| 12 | 240201214 | 欧阳文奇 | 注册 PR 只能新增 students/240201214/.student.yml |
| 13 | 240201106 | 曹敏 | 来源分支必须为 9 位学号 |
| 19 | 240201114 | 徐铭洋 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 20 | 240201209 | 黎绮雯 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 21 | 240201136 | 詹兴成 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 23 | 240201125 | 李明 | PR 作者与 github_username 不一致 |
| 24 | 240201226 | 杨文程 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 26 | 240201102 | 樊新妮 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 28 | 240201240 | 金佳诚 | 注册 PR 只能新增 students/240201240/.student.yml |
| 29 | 240201222 | 郭俊毅 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 30 | 240201204 | 龙玉新 | 来源分支必须为 9 位学号 |
| 31 | 240201224 | 钟逸飞 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 33 | 240201244 | 胡陈海 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 34 | 240201132 | 温子豪 | 来源分支必须为 9 位学号 |
| 36 | 240201115 | 章聪 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 38 | 240201107 | 沙明慧 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 41 | 240201127 | 敖文剑 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 42 | 240201238 | 钟祥明 | 来源分支必须为 9 位学号 |
| 44 | 240201215 | 查锦峰 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 45 | 240201219 | 张远哲 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 46 | 240201211 | 李昊泽 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 47 | 240201243 | 王文豪 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 49 | 240201245 | 薛子敬 | 注册 PR 只能新增 students/240201245/.student.yml |
| 50 | 240201217 | 杨跃 | 来源分支必须为 9 位学号 |
| 52 | 240201233 | 林博涵 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 53 | 240201235 | 黄嘉锋 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 54 | 240201232 | 林云智 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 55 | 240201234 | 陈幸 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 56 | 240201241 | 薛尔康 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 57 | 240201242 | 郭子弘 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 58 | 240201210 | 童怡玲 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 59 | 240201202 | 周佳桢 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 60 | 240201231 | 刘泽宇 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 61 | 240201221 | 王睿 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 63 | 240201205 | 余诗嘉 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 67 | 240201236 | 余坤 | 来源分支必须为 9 位学号 |
| 69 | 240201124 | 夏海彬 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 70 | 240201225 | 李浩 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 71 | 240201230 | 王晨曦 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 72 | 240201239 | 陈昭行 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 76 | 240201228 | 刘量 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 77 | 240201143 | 邢城铭 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 80 | 240201212 | 陈炎贵 | 来源分支必须为 9 位学号 |
| 85 | 240201133 | 肖焜 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 86 | 240201304 | 周懿 | students/240201304/.student.yml:1：应为顶格的 key: value |
| 87 | 240201140 | 余晖 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 89 | 240201334 | 郭昊 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 91 | 240201120 | 廖文旭 | 分支名、目录名和 student_id 必须相同 |
| 92 | 240201213 | 龙廷镐 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 93 | 240201325 | 陈志彬 | students/240201325/.student.yml:2：双引号字符串格式错误 |
| 94 | 240201312 | 葛李庆林 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 103 | 240201310 | 李家乐 | 注册 PR 只能新增 students/240201310/.student.yml |
| 108 | 240201427 | 金学忠 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 116 | 240201306 | 刘琴 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 120 | 240201339 | 丁志文 | students/240201339/.student.yml：必须包含 student_id、name、github_username |
| 124 | 240201331 | 曹俊恒 | 来源分支必须为 9 位学号 |
| 127 | 240201338 | 徐唐达 | students/240201338/.student.yml：必须包含 student_id、name、github_username |
| 131 | 240201346 | 程新南 | students/240201346/.student.yml：必须包含 student_id、name、github_username |
| 138 | 240201229 | 熊勋淏 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 141 | 240201110 | 汪夙夙 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 147 | 240201109 | 周敏 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 154 | 240201409 | 熊佳玲 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 157 | 240201410 | 李敏 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 160 | 240201409 | 熊佳玲 | 来源分支必须为 9 位学号 |
| 161 | 230201131 | 汤启浚 | 来源分支必须为 9 位学号 |
| 163 | 240201145 | 许欣杰 | 注册 PR 只能新增 students/240201145/.student.yml |
| 164 | 240201128 | 钟盛彬 | 注册 PR 只能新增 students/240201128/.student.yml |
| 165 | 240201117 | 李姚杰 | 注册 PR 只能新增 students/240201117/.student.yml |
| 166 | 240201131 | 黄武仪 | 注册 PR 只能新增 students/240201131/.student.yml |
| 173 | 240201106 | 曹敏 | 注册 PR 只能新增 students/240201106/.student.yml |
| 175 | 240201412 | 王子鸣 | 注册 PR 只能新增 students/240201412/.student.yml |
| 176 | 240201414 | 周健豪 | 来源分支必须为 9 位学号 |
| 177 | 240201103 | 吴金梅 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 178 | 240201411 | 彭东旭 | 注册 PR 只能新增 students/240201411/.student.yml |
| 179 | 240201422 | 滕昊 | 注册 PR 只能新增 students/240201422/.student.yml |
| 180 | 240201201 | 钱雨涵 | students/240201201/.student.yml：必须包含 student_id、name、github_username |
| 182 | 240201105 | 徐倩 | 来源分支必须为 9 位学号 |
| 184 | 240201428 | 钟晟 | 注册 PR 只能新增 students/240201428/.student.yml |
| 185 | 240201108 | 聂迪都 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 186 | 240201139 | 易芳斌 | 注册 PR 只能新增 students/240201139/.student.yml |
| 187 | 240201212 | 陈炎贵 | 首次注册只能新增一个 .student.yml，不能同时交作业或其他文件 |
| 188 | 240201121 | 刘永强 | 注册 PR 只能新增 students/240201121/.student.yml |
| 190 | 240201430 | 马谢俊 | 注册 PR 只能新增 students/240201430/.student.yml |
| 191 | 240201407 | 蒋欣亚 | 注册 PR 只能新增 students/240201407/.student.yml |
| 192 | 240201223 | 黄伟荣 | 注册 PR 只能新增 students/240201223/.student.yml |


# 以下同学未提交

| 学号 | 姓名 | 班级 |
| --- | --- | --- |
| 240201113 | 何丞鹏 | 2402011 |
| 240201130 | 单帆 | 2402011 |
| 240201138 | 彭小武 | 2402011 |
| 240201144 | 王昱文 | 2402011 |
| 240201218 | 万琪煜 | 2402012 |
| 240201237 | 曹子俊 | 2402012 |
| 240201311 | 宋阳 | 2402013 |
| 240201314 | 郑梓涵 | 2402013 |
| 240201317 | 陈浩东 | 2402013 |
| 240201324 | 刘璋毅 | 2402013 |
| 240201329 | 罗昌鸿 | 2402013 |
| 240201337 | 熊超 | 2402013 |
| 240201401 | 王晴晴 | 2402014 |
| 240201402 | 牛忻雅 | 2402014 |
| 240201413 | 卢巍中 | 2402014 |
| 240201415 | 江灿 | 2402014 |
| 240201416 | 秦可聪 | 2402014 |
| 240201417 | 曾鑫 | 2402014 |
| 240201418 | 吕乐 | 2402014 |
| 240201423 | 刘海旭 | 2402014 |
| 240201426 | 胡硕鸿 | 2402014 |
| 240201431 | 熊子杰 | 2402014 |
| 240201435 | 刘玉枫 | 2402014 |
| 240201436 | 洪世杰 | 2402014 |
| 240201437 | 郭程辉 | 2402014 |
| 240201438 | 陈俊杰 | 2402014 |
| 240201442 | 付畅畅 | 2402014 |
| 240201443 | 卢同乐 | 2402014 |
| 240201444 | 汪岸陆 | 2402014 |
| 240201446 | 王子懿 | 2402014 |
| 248201501 | 周耀宗 | 2482015 |
| 248201502 | 朱建超 | 2482015 |

## 第一次作业（HW01）：使用 Proteus 绘制电路原理图

### 1. 作业任务与参考电路

请每位同学独立使用 **Proteus**，根据下面的参考图片重新绘制一遍 **555 定时器与 4017 计数器电路**，完成元件放置、参数设置和导线连接，最后将自己绘制的原理图导出为 PDF。

![HW01 参考电路：555 定时器与 4017 计数器](assignments/HW01/reference.png)

**本次作业只需提交绘制好的电路原理图 PDF，不需要提交 Proteus 工程文件、PCB 文件、仿真结果、实验报告或压缩包。** 不要求完成仿真或制作实物；工程文件请自行保存在本地，便于修改后重新导出 PDF。

### 2. 绘制要求

- 必须在 Proteus 中自己放置元件、绘制连线，不能直接把参考图片粘贴进 PDF 作为作业。
- 元件数量、参数、电源与接地以及各引脚的连接关系应与参考图一致。
- 元件符号的外观和引脚排列可能与参考图不同，应按引脚编号及功能连接，不要只照着图形位置连线。
- 参考图中的元件标号与参数应清楚可见；检查连接点，避免把导线交叉误画成电气连接，或把应连接的位置画成断线。
- 可以适当调整布局，但应保持电路整洁、导线清楚、文字不重叠。
- 在图纸空白处注明本人姓名、学号和作业编号 `HW01`。

参考图中的主要元件与参数如下，连接关系以图片为准：

| 元件 | 数量 | 型号或参数 |
| --- | --- | --- |
| 555 定时器 | 1 | 555 |
| 4017 计数器 | 1 | 4017 |
| R1 | 1 | 10 kΩ |
| RV1 | 1 | 10 kΩ 可调电阻，注意滑动端连接 |
| R2、R3 | 2 | 各 680 Ω |
| C1 | 1 | 10 μF |
| C2 | 1 | 0.01 μF，即 10 nF |
| D1～D11 | 11 | 按图放置指示灯元件，注意极性 |
| 电源与接地 | 按图 | 电源标注 6～9 V，并绘制公共地 |

### 3. 导出与检查 PDF

绘制完成后先保存本地工程，再生成 PDF。支持直接导出的 Proteus 版本可在原理图的 **Output（输出）** 菜单中查找 PDF 导出选项；也可通过 **File → Printer Setup / Print（打印机设置／打印）** 选择 PDF 打印机输出。具体名称可能随版本和界面语言不同。[Proteus 官方入门教程：原理图 PDF 导出与打印](https://www.labcenter.com/downloads/Tutorials.pdf#page=53)

建议使用 A4 横向页面，调整比例，让整个电路完整呈现在一页中。导出后必须打开 PDF 检查：

- 电路完整，没有元件或导线被裁掉；
- 放大后，元件标号、参数和引脚编号仍然清楚；
- 姓名、学号和 `HW01` 标注正确；
- 文件不是空白页，也不是参考图片或软件界面的截图。

修改电路后，必须重新导出 PDF；只保存 Proteus 工程不会自动更新已导出的 PDF。

### 4. 提交文件、位置和 PR

PDF 文件统一命名为 `学号_HW01.pdf`，存放在 `students/本人学号/HW01/` 中。

例如学号为 `240201101`，本次作业只提交下面这一个文件：

```text
students/240201101/HW01/240201101_HW01.pdf
```

在自己的学号分支上，通过 Pull Request 提交至教师仓库 `rosickey/cad-homework-2026` 的 `main`。标题格式为：

```text
[240201101] HW01 - 王明
```

请替换为自己的学号和姓名。Git 操作见下文“三、提交电子线路 CAD 作业”。

> **首次注册和第一次作业是两个步骤。** 尚未注册的同学，先按下文“二、第一次提交”仅提交 `.student.yml`。等待注册 PR 合并后，再在同一学号分支提交 HW01 的 PDF 并新建作业 PR。已注册的同学无需重复提交或修改身份文件。

## 一、Windows 准备工作

### 1. 注册并登录 GitHub

打开 <https://github.com> 注册个人账号，并完成邮箱验证。

请记住自己的 **GitHub 用户名**。例如个人主页是：

```text
https://github.com/wangming123
```

则 GitHub 用户名是：

```text
wangming123
```

用户名不是页面显示的中文昵称，也不是邮箱地址。

### 2. 安装 Git for Windows

1. 打开 Git 官方下载页面：<https://git-scm.com/download/win>；
2. 下载适合自己电脑的安装程序。大多数 Windows 10/11 电脑选择 **64-bit Git for Windows Setup**；
3. 双击安装程序；
4. 一般保持默认选项即可；
5. 安装组件时保留 **Git Bash Here**；
6. 凭据管理选项保留 **Git Credential Manager**；
7. 完成安装。[Git for Windows 视频教程](https://www.bilibili.com/video/BV1LUKk6wEWr)

如果安装程序要求选择默认编辑器，不熟悉 Vim 的同学可以选择 **Notepad**、**Notepad++** 或已经安装的 **Visual Studio Code**。

安装完成后，从开始菜单打开：

```text
Git Bash
```

输入：

```bash
git --version
```

如果看到类似下面的版本信息，说明安装成功：

```text
git version 2.x.x.windows.x
```

如果提示 `git: command not found`，请关闭当前窗口，重新打开 Git Bash；仍然无效时重新安装 Git for Windows。

### 3. 认识 Git Bash

Git Bash 是本课程推荐使用的 Git 命令行。打开方式有两种：

- 在 Windows 开始菜单搜索并打开 **Git Bash**；
- 在文件夹空白处单击右键，选择 **Open Git Bash here** 或 **Git Bash Here**。Windows 11 有时需要先点击“显示更多选项”。

Git Bash 中常用的基础命令：

| 命令 | 作用 |
| --- | --- |
| `pwd` | 显示当前所在目录 |
| `ls` | 查看当前目录中的文件 |
| `ls -la` | 查看全部文件，包括以 `.` 开头的隐藏文件 |
| `cd 文件夹名` | 进入指定文件夹 |
| `cd ..` | 返回上一级目录 |
| `mkdir 文件夹名` | 创建文件夹 |
| `clear` | 清理终端显示 |

例如进入 Windows 的 `D:\course` 文件夹，在 Git Bash 中可以写：

```bash
cd /d/course
```

Windows 路径和 Git Bash 路径的对应关系示例：

```text
C:\Users\wang\Desktop  →  /c/Users/wang/Desktop
D:\course              →  /d/course
```

路径中如果包含空格，需要加英文双引号：

```bash
cd "/d/CAD Course"
```

粘贴命令时可以使用右键、`Shift+Insert`，或者在新版 Git Bash 中使用 `Ctrl+Shift+V`。不要把命令提示符 `$` 一起复制进去。

### 4. 第一次配置 Git

下面两项只需在自己的电脑上设置一次：

```bash
git config --global user.name "你的姓名"
git config --global user.email "你的GitHub邮箱"
```

例如：

```bash
git config --global user.name "王明"
git config --global user.email "wangming@example.com"
```

检查配置：

```bash
git config --global --list
```

这里的姓名和邮箱会记录在 Git 提交中。建议使用已添加到 GitHub 账号的邮箱；如果不希望公开真实邮箱，也可以使用 GitHub 提供的 `noreply` 邮箱。

### 5. 选择本地课程文件夹

建议在磁盘中建立一个路径简单、没有中文和特殊符号的课程目录，例如：

```text
D:\course
```

然后在该文件夹中打开 Git Bash，或者执行：

```bash
cd /d/course
```

后面的 Clone 命令会在这里自动创建课程仓库文件夹。

## 二、第一次提交：注册学号与 GitHub 用户名

第一次 PR **只注册身份，不提交作业 PDF**。教师审核并合并后，学号与 GitHub 用户名即完成绑定，再按作业要求提交 HW01。

### 1. Fork 课程仓库

登录自己的 GitHub 账号，打开课程仓库，点击右上角的 **Fork**，将仓库复制到自己的账号下。

例如 GitHub 用户名为 `wangming123`，Fork 后的仓库是：

```text
https://github.com/wangming123/cad-homework-2026
```

### 2. Clone 自己的 Fork

把下面命令中的 `你的GitHub用户名` 替换为自己的用户名：

```bash
git clone https://github.com/你的GitHub用户名/cad-homework-2026.git
cd cad-homework-2026
```

第一次连接 GitHub 时，浏览器或 Git Credential Manager 可能要求登录授权。请使用自己的 GitHub 账号完成登录，不要输入其他同学的账号。[GitHub Fork 操作说明视频](https://www.bilibili.com/video/BV1bd4y1J7Vt)

Clone 完成后，可以用下面的命令确认当前位置和仓库内容：

```bash
pwd
ls -la
git status
```

### 3. 添加教师仓库为 upstream

```bash
git remote add upstream https://github.com/rosickey/cad-homework-2026.git
git remote -v
```

其中：

- `origin` 是你自己的 Fork；
- `upstream` 是教师的课程仓库。

### 4. 创建学号分支

先取得教师仓库的最新内容，再创建以完整学号命名的分支：

```bash
git fetch upstream
git switch main
git pull --ff-only upstream main
git switch -c 240201101
```

请把示例学号 `240201101` 替换为你自己的 9 位学号。

检查当前分支：

```bash
git branch --show-current
```

输出必须是你自己的完整学号。不要使用 `HW01`、`姓名-HW01` 或 `学号-HW01` 作为分支名。

### 5. 创建身份文件

创建自己的目录：

```bash
mkdir -p students/240201101
```

先创建空的身份文件，再用 Windows 记事本打开：

```bash
touch students/240201101/.student.yml
notepad students/240201101/.student.yml
```

如果记事本询问是否创建新文件，选择“是”。也可以使用 Visual Studio Code 等纯文本编辑器打开该文件。

文件位置为：

```text
students/240201101/.student.yml
```

文件内容如下：

```yaml
student_id: "240201101"
name: "王明"
github_username: "wangming123"
```

保存后执行：

```bash
ls -la students/240201101
```

必须能看到准确的文件名 `.student.yml`。如果显示为 `.student.yml.txt`，说明保存格式错误，请先改回 `.student.yml`，否则无法注册。

请替换为自己的真实信息：

- `student_id`：9 位完整学号，必须与分支名、目录名一致；
- `name`：真实姓名；
- `github_username`：GitHub 用户名，不是昵称，也不是邮箱。

例如 GitHub 主页地址是 `https://github.com/wangming123`，用户名就是 `wangming123`。

### 6. 检查、提交并 Push

第一次 PR 只能包含自己的 `.student.yml`：

```bash
git status
git add students/240201101/.student.yml
git commit -m "register 240201101 王明"
git push -u origin 240201101
```

请将命令中的学号和姓名替换为自己的信息。

### 7. 创建第一次 Pull Request

打开自己 Fork 后的仓库，点击 **Compare & pull request**，确认：

```text
base repository: rosickey/cad-homework-2026
base branch:     main
head repository: 你的GitHub用户名/cad-homework-2026
compare branch:   你的学号
```

PR 标题统一写为：

```text
[REGISTER] 240201101 王明
```

教师将核对：

1. PR 提交者是否为本人 GitHub 账号；
2. 分支、目录和 `student_id` 是否为同一个学号；
3. `github_username` 是否与 PR 提交者一致；
4. PR 是否只新增自己的 `.student.yml`。

审核通过并合并后，绑定关系固定为：

```text
GitHub 用户名 ↔ 学号 ↔ 学号分支 ↔ 学号目录
```

注册完成后，学生不得自行修改或删除 `.student.yml`。如姓名、学号或 GitHub 用户名确需变更，请联系教师。

## 三、提交电子线路 CAD 作业

整个课程期间继续使用同一个学号分支，不要为每次作业另建分支，也不要删除该分支。

### 1. 同步教师仓库

先在本地 `cad-homework-2026` 文件夹中打开 Git Bash，再执行以下命令。如果终端当前位于该文件夹的上一级，先执行 `cd cad-homework-2026`；已经在仓库内时不需要重复执行 `cd`。

```bash
git status
git fetch upstream
git switch 240201101
git merge --no-edit upstream/main
```

将 `240201101` 替换为自己的学号。

同步前如 `git status` 显示尚未处理的改动，先确认并保存自己的工作。如果 Git 提示存在冲突，不要随意删除文件，请保留终端提示并联系教师。

### 2. 创建作业目录

例如提交 HW01：

```bash
mkdir -p students/240201101/HW01
```

本次 **HW01 只需将从 Proteus 导出的原理图 PDF** 放入该目录，文件名为 `240201101_HW01.pdf`。不要把本地 Proteus 工程、自动备份和临时文件一并复制到提交目录中。

以学号 `240201101` 为例，注册文件和作业文件用途如下：

| 文件路径 | 用途 |
| --- | --- |
| `students/240201101/.student.yml` | 已合并的身份文件，保留不动 |
| `students/240201101/HW01/240201101_HW01.pdf` | 本次作业唯一需要新增或更新的提交文件 |

后续作业的提交格式以对应作业布置为准；本说明不统一要求上传 CAD 工程文件。本地工程请自行保存，不要因本次不要求上传而删除。

### 3. 提交作业

```bash
git status
git diff
git add students/240201101/HW01/240201101_HW01.pdf
git diff --cached --name-only
git commit -m "240201101 HW01"
git push origin 240201101
```

`git diff --cached --name-only` 用于确认本次准备提交的文件。本次 HW01 应只列出自己的 `学号_HW01.pdf`，如出现其他文件，先停止提交并检查。PDF 可能只显示二进制文件发生变化，图纸质量需要通过打开 PDF 检查。

提交前必须确认所有改动都位于：

```text
students/自己的学号/
```

### 4. 创建作业 PR

PR 仍然从自己的学号分支提交到教师仓库的 `main`：

```text
自己的学号 → main
```

标题格式：

```text
[240201101] HW01 - 王明
```

全班注册结束、教师启用检查后，提交作业将运行自动检查，并等待教师审核。自动检查主要验证：

- PR 作者及 Fork 所有者是否与绑定的 GitHub 用户名一致；
- 分支名是否为本人学号；
- 是否只修改 `students/本人学号/`；
- 是否修改或删除了 `.student.yml`；
- 重命名前后的路径是否都属于本人目录。

自动检查通过不代表图纸内容合格，电路绘制和 PDF 提交内容仍由教师审核。如果上一份 PR 还没有合并，同一分支的新提交会加入该 PR，请不要将下一次作业提前混入。

## 四、教师要求修改时

如果教师在尚未合并的 PR 中提出修改意见，不要新建 PR。在 Proteus 中修改电路并重新导出 PDF，替换自己的原 PDF 后，继续提交到同一学号分支：

```bash
git status
git add students/240201101/HW01/240201101_HW01.pdf
git diff --cached --name-only
git commit -m "240201101 HW01 fix"
git push origin 240201101
```

原 PR 会自动更新；已启用的自动检查也会重新运行。

## 五、常见问题和检查错误

### Windows 和 Git 常见问题

| 现象 | 处理方法 |
| --- | --- |
| `git` 不是内部或外部命令 | 请在 Git Bash 中执行；确认 Git for Windows 已安装后重新打开终端 |
| `cd` 后提示目录不存在 | 先执行 `pwd`、`ls` 检查位置；含空格的路径要加英文双引号 |
| `.student.yml` 看不到 | 执行 `ls -la students/自己的学号`；以 `.` 开头的文件通常被隐藏 |
| 文件实际变成 `.student.yml.txt` | 在资源管理器中开启“显示文件扩展名”，删除末尾的 `.txt` |
| Clone 或 Push 时要求登录 | 按 Git Credential Manager 或浏览器提示登录自己的 GitHub 账号 |
| Push 显示无权限 | 确认 `origin` 是自己 Fork 的仓库，可执行 `git remote -v` 检查 |
| 电路已修改，但 PDF 或 Git 没变化 | 在 Proteus 中重新导出 PDF，保存到本人 HW01 提交路径，再执行 `git status` |
| `git diff` 只显示二进制文件变化 | PDF 的常见显示方式；自行打开 PDF 检查电路，并用 `git diff --cached --name-only` 核对提交文件 |

### 自动检查错误

| 检查提示 | 原因 | 处理方法 |
| --- | --- | --- |
| `Unknown student ID` | 学号尚未绑定，或分支名错误 | 检查分支名；如尚未注册，联系教师 |
| `GitHub username does not match` | PR 用户与已绑定账号不同 | 使用本人已绑定的 GitHub 账号 |
| `Head repository owner does not match` | PR 来源 Fork 不属于已绑定账号 | 从本人 Fork 的学号分支提交 |
| `Unauthorized path` | 修改了本人目录以外的文件 | 撤销越界修改后再次 Push |
| `Registration file is locked` | 修改或删除了 `.student.yml` | 恢复该文件；需变更身份时联系教师 |

不要重复创建 PR。修正本地文件后 `commit`、`push`，原 PR 会自动更新。

## 六、每次提交前检查

- [ ] 登录的是自己的 GitHub 账号；
- [ ] 当前分支是自己的 9 位学号；
- [ ] 只修改了 `students/自己的学号/`；
- [ ] 注册通过后没有修改 `.student.yml`；
- [ ] 没有修改其他学生或课程公共文件；
- [ ] 已执行 `git status` 并核对暂存文件清单；
- [ ] HW01 只提交 `students/本人学号/HW01/学号_HW01.pdf`；
- [ ] PDF 是自己使用 Proteus 绘制的电路，不是参考图片；
- [ ] 已打开 PDF 检查完整性、清晰度以及姓名和学号；
- [ ] PR 目标仓库为 `rosickey/cad-homework-2026`；
- [ ] PR 目标分支为 `main`；
- [ ] 教师启用自动检查后，相关检查已经通过。

## 七、最常用命令

```bash
# 查看当前分支
git branch --show-current

# 查看修改状态
git status

# 同步教师仓库
git fetch upstream
git switch 240201101
git merge --no-edit upstream/main

# 提交并上传
git add students/240201101/HW01/240201101_HW01.pdf
git diff --cached --name-only
git commit -m "240201101 HW01"
git push origin 240201101
```

请把所有示例中的 `240201101` 替换为自己的真实学号。
