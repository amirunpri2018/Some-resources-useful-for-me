# jupyter config

## jupyter notebook can not open browser self

[https://support.anaconda.com/customer/en/portal/articles/2925919-change-default-browser-in-jupyter-notebook](https://support.anaconda.com/customer/en/portal/articles/2925919-change-default-browser-in-jupyter-notebook)

## jupyter themes

* 终端配置

```bash
jt -t onedork -fs 11 -nfs 11
```

* notebook 配置

```python
# import jtplot module in notebook
from jupyterthemes import jtplot

# choose which theme to inherit plotting style from
# onedork | grade3 | oceans16 | chesterish | monokai | solarizedl | solarizedd
jtplot.style(theme='onedork')

# set "context" (paper, notebook, talk, poster)
# scale font-size of ticklabels, legend, etc.
# remove spines from x and y axes and make grid dashed
jtplot.style(context='talk', fscale=1.4, spines=False, gridlines='--')

# turn on X- and Y-axis tick marks (default=False)
# turn off the axis grid lines (default=True)
# and set the default figure size
jtplot.style(ticks=True, grid=False, figsize=(6, 4.5))

# reset default matplotlib rcParams
jtplot.reset()
```

## 行号显示

在 “查看” 中 “切换行号”


