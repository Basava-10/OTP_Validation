# OTP_Validation
from random import randint
correct_otp= randint(100000,999999)
print(correct_otp)
for attempt in range(1,3):
    user_input=input(f"Attempt {attempt}: Enter OTP:")
    if user_input==str(correct_otp):
        print("OTP verification successful: Access granted😊")
        break
    else:
        print("Incorrect OTP.Try again :)")
else:
    print("Maximum attempts reached.Your Account locked")
