from tkinter import*
from tkinter.ttk import*

from time import strftime

root = Tk()
root.title("clock")

def time():
    string = strftime('%H:%M:%S %p')
    label.config(text=string)
    label.after(1000, time)

label = Label(root, font=("ds-digital", 80), background = "black", foreground = "pink")
label.pack(anchor='center')
time()

mainloop()
.
.
.
THE RAINMETER FOR CLOCK
[ds_digital.zip](https://github.com/matejgec/matejgec/files/8643306/ds_digital.zip)
