# hotel-mainu

mainu = {
    'BIRYANI': 200,
    'DOSA': 50,
    'CHIKAN': 150,
    'CHHOLE': 50,
}

print("WELCOME TO SAMMY RESTAURANT")
print("BIRYANI : RS200")
print("DOSA     : RS50")
print("CHIKAN   : RS150")
print("CHHOLE   : RS50")

order_total = 0

o = input("Enter your order: ").upper()

if o in mainu:
    order_total += mainu[o]
    print(f"{o} has been added.")
else:
    print(f"{o} is not available.")

o1 = input("Do you want another order? (yes/no): ").lower()

if o1 == "yes":
    o0 = input("Enter your second order: ").upper()

    if o0 in mainu:
        order_total += mainu[o0]
        print(f"{o0} has been added.")
    else:
        print(f"{o0} is not available.")

print(f"Your total bill is Rs {order_total}")
