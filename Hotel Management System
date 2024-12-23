def show_rooms():
    print("\nWelcome to King Hotel")
    print("1. Single Room - Rs. 1500")
    print("2. Double Room - Rs. 3000")
    print("3. Executive Suite - Rs. 7500")
    print("4. Premium Suite - Rs. 10000")
    print()

def book_room():

    name = input("Enter your name: ")
    try:
        nights = int(input("How many nights? "))
        room_type = int(input("Choose room (1, 2, 3, 4): "))
    except:
        print("Invalid input!")
        return

    if room_type == 1:
        room = "Single Room"
        cost = 1500
    elif room_type == 2:
        room = "Double Room"
        cost = 3000
    elif room_type == 3:
        room = "Executive Suite"
        cost = 7500
    elif room_type == 4:
        room = "Premium Suite"
        cost = 10000
    else:
        print("Wrong room type!")
        return

    total = cost * nights
    print("\nBooking Details:")
    print("Name:", name)
    print("Room:", room)
    print("Nights:", nights)
    print("Total Cost: Rs.", total)
    print("Thank you for Booking \n")

def cancle_booking():
    name = input("\nEnter name for cancelling: ")
    print("Booking cancelled for", name, "\n")

def main():
    while True:
        print("\nHotel System")
        print("1. Show Rooms")
        print("2. Book Room")
        print("3. Cancel Room")
        print("4. Exit")
        try:
            choice = int(input("Enter choice: "))
        except:
            print("Enter a number")
            continue

        if choice == 1:
            show_rooms()
        elif choice == 2:
            book_room()
        elif choice == 3:
            cancle_booking()
        elif choice == 4:
            print("Thank you for visiting...Byee")
            break
        else:
            print("Wrong choice\n")

main()
