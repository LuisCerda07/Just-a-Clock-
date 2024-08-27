import tkinter as tk
from datetime import datetime


def update_label():

    time_now = datetime.now().time()
    time_sys = time_now.strftime('%H:%M')

    c_label.config(text = time_sys)
    window.after(1000, update_label)

    return

window = tk.Tk()
window.title("Just a Clock!")
window.geometry("400x250")
window.configure(bg = "gray")
window.resizable(False, False)


l_button = tk.Button(window, text = "", bg = "red", activebackground = "#800000", width= 17, bd = 5,) 
l_button.grid(row = 0, column = 0, sticky="w", padx = 59, pady = 20)

r_button = tk.Button(window, text = "", bg = "red", activebackground = "#800000", width= 17, bd = 5)
r_button.grid(row = 0, column = 0, sticky="w", padx = 202, pady = 20)

c_label = tk.Label(window, text = "", font = ("Fixedsys", 50), width = 7, height = 2, borderwidth = 3, relief = "solid")
c_label.grid(column = 0, row = 1, sticky = "w", padx = 55, pady = 0)


update_label()
window.mainloop()

