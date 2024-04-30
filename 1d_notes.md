# Python 1

problems with 1d_demo2.py

Using matplotlib

Needs an appropriate backend defined in matplotlibrc (where is it?)
To find the matplotlibrc that is in use, from a terminal:

```
python3
>>> import matplotlib
>>> matplotlib.matplotlib_fname()
```
Need sudo to edit matplotlibrc; this works for me and on ubuntu the QT backend is nicer I think (easy to label graph etc)

```
## ***************************************************************************
## * BACKENDS                                                                *
## ***************************************************************************
## The default backend.  If you omit this parameter, the first working
## backend from the following list is used:
##     MacOSX QtAgg Gtk4Agg Gtk3Agg TkAgg WxAgg Agg
## Other choices include:
##     QtCairo GTK4Cairo GTK3Cairo TkCairo WxCairo Cairo
##     Qt5Agg Qt5Cairo Wx  # deprecated.
##     PS PDF SVG Template
## You can also deploy your own backend outside of Matplotlib by referring to
## the module name (which must be in the PYTHONPATH) as 'module://my_backend'.
backend: Qt5Agg
```
Also the file 1d_demo2.py as furnished omitted a line needed to display:
`plt.show()`

## Python syntax
formatted print uses
`print(f"Hello {variable}")`

Lists defined by `list = [1,a,3,b,5,c]`

Access list by position for reading or writing, `list[2]` is the third item in the list (lists start at 0). `list[-1]` is the last item.


