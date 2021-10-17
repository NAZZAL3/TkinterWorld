#Graphical User Interfaces
from tkinter import *
from tkinter import colorchooser


def click():
    color = colorchooser.askcolor() #Make a Var called Color the gave it '.ask Color()'
    colorHex = color[1]  #Creat the HexDecimal Value 
    print(colorHex)
    window.config(bg=colorHex)#Change The Background Color To A HexDecimle.


window = Tk() #Window 'Most Important IS Tk()'
window.geometry('420x420') #Set Screen Resulotion.
button_me = Button(text='Color Picker!', command=click, padx=12, pady=10) #Creat Button
button_me.pack() 


window.mainloop()
