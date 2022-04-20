This fork allows us to create Tk() windows and assign style manager to them as we can do in tkinter.ttk

Example:

```python
  from tkinter import *
  from ttkbootstrap import *
  
  
  def display_window2():
    window2 = Tk()
    style2 = Style(window2)
    style2.theme_use('flatly')
  
    button2 = Button(window2, text='Nothing')
    button2.pack()
  
    
    
  window1 = Tk()
  style1 = Style(window1)
  style1.theme_use('cosmo')
  
  button1 = Button(window1, text='display window2', command=display_window2)
  button1.pack()
  
  window1.mainloop()
```
