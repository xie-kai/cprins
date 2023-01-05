# cprints

##  安装说明

使用`pip`或其他 PyPi 软件包进行安装

```
pip install cprints
```

## 使用 cprints 输出彩色文本

您可以试试：

```python
from cprints import cp


# 红色文字 文字样式: 下划线
cp.print_red("Hello World", style=cp.underline)

# 绿色文字 红色背景
cp.print_green("Hello World", bg="red")

# 黄色文字 黑色背景 文字样式: 下换线 and 高亮
cp.cprint(
    "Hello World",
    fg="yellow",
    bg=cp.black,
    style=["underline", "高亮"]
)

# color着色文字
# 黑色文字 白色背景 文字样式: 反显
text = cp.color("Hello World", fg=cp.black, bg=cp.white, style=cp.reverse)
print(text)
```
