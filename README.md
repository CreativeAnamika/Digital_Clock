# Digital_Clock
#We are having a digital clock(a very small project!!!
import tkinter as tk
import time import strftime
 
 
root=tk.TK()
root.title("Digital Clock")

def time():
    string=strftime('%H:%M%S %P \n %D') 
    label.config(text=string)
    label.after(1000,time)
    
label=tk.label(root,font=('calibri',50,'bold'),background='yellow',foreground='black')    
label.pack(anchor='center')

time()

root.mainloop()
