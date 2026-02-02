# EXERCISE-BY-ILLUSTRATING-REGULAR-EXPRESSION
import re
phone = input("Enter your phone number (format XXX-XXX-XXXX): ")
phone_pattern = r"^\d{3}-\d{3}-\d{4}$"
if re.match(phone_pattern, phone):
    print("Phone number is valid!")
else:
    print(" Invalid phone number format!")

password = input("Enter your password: ")
password_pattern = r"^(?=.*[a-z])(?=.*[A-Z])(?=.*\d).{8,}$"
if re.match(password_pattern, password):
    print("Strong password!")
else:   
    print("Weak password! Make sure it has at least 8 characters, including:")
    print("   - 1 uppercase letter")
    print("   - 1 lowercase letter")
    print("   - 1 digit")

Output:

Enter your phone number (format XXX-XXX-XXXX): 999-985-9234
Phone number is valid!
Enter your password: psgr@123
Weak password! Make sure it has at least 8 characters, including:
   - 1 uppercase letter
   - 1 lowercase letter
   - 1 digit











