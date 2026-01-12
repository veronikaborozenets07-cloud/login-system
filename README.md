correct_username = "admin"
correct_password = "1234"

attempts = 0
logged_in = False

while attempts < 3 and not logged_in:
    username = input("Enter username: ")
    password = input("Enter password: ")

    if username == correct_username and password == correct_password:
        logged_in = True
        print("Login successful!")
    else:
        attempts += 1
        print("Wrong login or password.")

if not logged_in:
    print("Too many attempts. Access denied.")
# login-system
