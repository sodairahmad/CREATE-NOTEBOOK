# CREATE tabs
how to create notebook and tabs  in tkinter and some other functions

code()
from tkinter import *
from tkinter import ttk

window= Tk()

notebook=ttk.Notebook(window)

Tab1=Frame(notebook)
Tab2=Frame(notebook)

notebook.add(Tab1,text="tab1")
notebook.add(Tab2,text="tab2")
notebook.pack(expand=True,fill='both')

Label(Tab1,text="this is tab1 note book",width=50,height=10,font="bold").pack()
Label(Tab2,text="this is tab2 note book",width=50,height=10,font="bold").pack()


window.mainloop()

END().......................................................................

TITLE=(HOE TO CEATE GEOMETRIC LABELS IN PYTHON)
CODE
from tkinter import *
window= Tk()

enterInfo=Label(window,text="Enter your info",font=("bold",35)).grid(row=0,column=0,columnspan=2)
enterFirstName=Label(window,text="enter your first name",width=20,bg='red',bd=2,font='5').grid(row=1,column=0)
entry=Entry(window,font='5').grid(row=1,column=1)
enterLastName=Label(window,text="enter your last name",width=20,bg='green',bd=2,font='5').grid(row=2,column=0)
entry=Entry(window,font='5').grid(row=2,column=1)
enterEmail=Label(window,text="enter your Email",width=20,bg='blue',bd=2,font='5').grid(row=3,column=0)
entry=Entry(window,font='5').grid(row=3,column=1)


window.mainloop()
END()...........................................................................

title(how to create progress bar in python)
code
from tkinter import *
from tkinter.ttk import *
import time
def start():
    tasks=10
    x=0
    while(x<tasks):
        time.sleep(1)
        bar['value']+=10
        x+=1
        percent.set(str(int((x / tasks) * 100))+ '%')
        text.set(str(x)+"/"+str(tasks)+" tasks are completed")
        window.update_idletasks()


window=Tk()
percent=StringVar()
text=StringVar()
bar=Progressbar(window,length=300)
bar.pack(pady=10)
percentshow=Label(window,textvariable=percent).pack()
taskshow=Label(window,textvariable=text).pack()

button=Button(text="download",command=start)
button.pack()

window.mainloop()

END()...................................................................

TITLE(HOW TO CREATE SHAPES IN PYTHON USING CANVAS)
CODE
from tkinter import *

window= Tk()

canvas=Canvas(window,height=400,width=400)
canvas.create_line(0,0,400,400,fill='red',width=5)
canvas.create_line(0,400,400,0,fill='blue',width=5)
canvas.create_rectangle(250,250,130,90,fill='red')
canvas.create_arc(90,90,200,200, fill='black',extent=90)
canvas.create_polygon(200,0,150,60,270,60,fill='yellow')
canvas.create_oval(130,160,200,230,fill='green')
canvas.pack()



window.mainloop()

END()...............................................................

TITLE()
