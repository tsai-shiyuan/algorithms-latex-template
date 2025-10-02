# 算法作业模板

这是一个算法课作业模版. 主要引入了和伪代码相关的包, 并且把题目的答案放到不同的文件, 便于书写~

## 文件介绍

- `main.tex` 主文件
- `template.tex` 配置文件
- `problem.tex` 自己的题解
- `figures` 图片文件夹

## 使用方法

在 template.tex 中填写个人信息和作业信息:

```tex
% 个人信息 
\newcommand{\myId}{23378888}
\newcommand{\myName}{灰太狼}

% 作业信息
\newcommand{\myHomeworkId}{1}
```

引入新的 `.tex` 文件, 需要在 `main.tex` 中添加:

```tex
\input{problem.tex}
```

使用 xelatex 编译. 运行命令:

```bash
xelatex -synctex=1 -interaction=nonstopmode main.tex
```

或者在 VSCode 中点击 Recipe: latexmk (xelatex) 
