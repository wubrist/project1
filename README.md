# project1
Ticket__Machine
from datetime import time

c = 0
m = 0
p = 0


def darug_stor():
    if visit == "cosmetic":
        global c
        c += 1
        print(f"c_{c}")

    if visit == "perfumes":
        global p
        p += 1
        print(f"p_{p}")
    if visit == "medicine":
        global m
        m += 1
        print(f"m_{m}")


id_list = [12346, 223467]
count = 0
count_limit = 3

while count_limit > count:
    id_number = int(input("please enter your id number:"))
    if id_number in id_list:
     import time

    t = input("Enter the time in seconds: ")
    while t:
        mins, secs = divmod(t, 60)
        timeformat = "{:02d}:{:02d}".format(mins,secs)
        print(timeformat)
        time.sleep(1)
        t -= 1

    visit = (input("please enter your visit:"))
    while visit != "":
        print("your number is:")
        darug_stor()
        print("please wait some one to assist you:")
        permission = input("do yuo want to continue ?Y/N")
        if permission == "y":
            visit = input("please enter your visit:")
        else:

            print()
            exit(0)

    count += 1
else:
    print("your choose is incorrect password")
    print("Done")


