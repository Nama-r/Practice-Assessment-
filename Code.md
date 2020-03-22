# Practice-Assessment-

# the variables are set (the size of the drinks and price)
small_drink_price = int(3)
medium_drink_price = int(4.5)
large_drink_price = int(6)

class Invalid(Exception):
    pass
class InvalidDrinkSelection(Invalid):
    pass
class InvalidConfirmation(Invalid):
    pass
class InvalidSize(Invalid):
    pass

drinks = []

# a function is created 
def drink_selection():
    while True:
        try: 
# flavours of the drinks are displayed where you get a choice for your selection            
            print("\nToday's Drink Options:\n1. Apple & Orange\n2. Mango\n3. Mixed Berries\n4. Tropical")
            chosen_drink = input("Choose which drink you would like by entering the number: ") 
            # if drink 1 is chosen which is apple and orange then this code runs 
            if chosen_drink == "1":
                print("\nAll drinks come in\n1. Small\n2. Medium\n3. Large")
                while True:
                    size = input("Choose what size you would like by entering the number: ").strip().lower()
                    try: 
# if small size is chosen this code runs 
                        if size == "1":
                            while True:
                                size_confirmation = input("\nWould you like to add a Small Apple & Orange drink to your order? (Yes or No): ").strip().lower()
                                try:
                                    if size_confirmation == "yes":
                                        drinks.append("- Small Apple & Orange")
                                        return
                                    elif size_confirmation == "no":
                                        drink_selection()
                                    else:
                                        raise InvalidConfirmation
                                except InvalidConfirmation:
                                    print("Please input a valid answer (Either 'Yes' or 'No').") 
 # if size medium is chosen this code runs 
                        elif size == "2":
                            while True:
                                size_confirmation = input("\nWould you like to add a Medium Apple & Orange drink to your order? (Yes or No): ").strip().lower()
                                try:
                                    if size_confirmation == "yes":
                                        drinks.append("- Medium Apple & Orange")
                                        return
                                    elif size_confirmation == "no":
                                        drink_selection()
                                    else:
                                        raise InvalidConfirmation
                                except InvalidConfirmation:
                                    print("Please input a valid answer (Either 'Yes' or 'No').") 
# if size large is chosen this code runs 
                        elif size == "3":
                            while True:
                                size_confirmation = input("\nWould you like to add a Large Apple & Orange drink to your order? (Yes or No): ").strip().lower()
                                try:
                                    if size_confirmation == "yes":
                                        drinks.append("- Large Apple & Orange")
                                        return
                                    elif size_confirmation == "no":
                                        drink_selection()
                                    else:
                                        raise InvalidConfirmation
                                except InvalidConfirmation:
                                    print("Please input a valid answer (Either 'Yes' or 'No')")
                        else:
                            raise InvalidSize
                    except InvalidSize:
                        print("\nPlease input a valid number (1 - 3).")                
            elif chosen_drink == "2":
                print("All drinks come in\n1. Small\n2. Medium\n3. Large")
                while True:
                    size = input("Choose what size you would like by entering the number: ").strip().lower()
                    try:
                        if size == "1":
                            while True:
                                size_confirmation = input("\nWould you like to add a Small Mango drink to your order? (Yes or No): ").strip().lower()
                                try:
                                    if size_confirmation == "yes":
                                        drinks.append("- Small Mango")
                                        return
                                    elif size_confirmation == "no":
                                        drink_selection()
                                    else:
                                        raise InvalidConfirmation
                                except InvalidConfirmation:
                                    print("Please input a valid answer (Either 'Yes' or 'No').")
                        elif size == "2":
                            while True:
                                size_confirmation = input("\nWould you like to add a Medium Mango drink to your order? (Yes or No): ").strip().lower()
                                try:
                                    if size_confirmation == "yes":
                                        drinks.append("- Medium Mango")
                                        return
                                    elif size_confirmation == "no":
                                        drink_selection()
                                    else:
                                        raise InvalidConfirmation
                                except InvalidConfirmation:
                                    print("Please input a valid answer (Either 'Yes' or 'No').")
                        elif size == "3":
                            while True:
                                size_confirmation = input("\nWould you like to add a Large Mango drink to your order? (Yes or No): ").strip().lower()
                                try:
                                    if size_confirmation == "yes":
                                        drinks.append("- Large Mango")
                                        return
                                    elif size_confirmation == "no":
                                        drink_selection()
                                    else:
                                        raise InvalidConfirmation
                                except InvalidConfirmation:
                                    print("Please input a valid answer (Either 'Yes' or 'No')")
                        else:
                            raise InvalidSize
                    except InvalidSize:
                        print("\nPlease input a valid size (Either 'Small', 'Medium' or 'Large')")                
            elif chosen_drink == "3":
                print("\nPlease input a valid number (1 - 3).")
                while True:
                    size = input("Choose what size you would like by entering the number: ").strip().lower()
                    try:
                        if size == "1":
                            while True:
                                size_confirmation = input("\nWould you like to add a Small Mixed Berries drink to your order? (Yes or No): ").strip().lower()
                                try:
                                    if size_confirmation == "yes":
                                        drinks.append("- Small Mixed Berries")
                                        return
                                    elif size_confirmation == "no":
                                        drink_selection()
                                    else:
                                        raise InvalidConfirmation
                                except InvalidConfirmation:
                                    print("Please input a valid answer (Either 'Yes' or 'No').")
                        elif size == "2":
                            while True:
                                size_confirmation = input("\nWould you like to add a Medium Mixed Berries drink to your order? (Yes or No): ").strip().lower()
                                try:
                                    if size_confirmation == "yes":
                                        drinks.append("- Medium Mixed Berries")
                                        return
                                    elif size_confirmation == "no":
                                        drink_selection()
                                    else:
                                        raise InvalidConfirmation
                                except InvalidConfirmation:
                                    print("Please input a valid answer (Either 'Yes' or 'No').")
                        elif size == "3":
                            while True:
                                size_confirmation = input("\nWould you like to add a Large Mixed Berries drink to your order? (Yes or No): ").strip().lower()
                                try:
                                    if size_confirmation == "yes":
                                        drinks.append("- Large Mixed Berries")
                                        return
                                    elif size_confirmation == "no":
                                        drink_selection()
                                    else:
                                        raise InvalidConfirmation
                                except InvalidConfirmation:
                                    print("Please input a valid answer (Either 'Yes' or 'No')")
                        else:
                            raise InvalidSize
                    except InvalidSize:
                        print("\nPlease input a valid number (1 - 3).")                
            elif chosen_drink == "4":
                print("All drinks come in\n1. Small\n2. Medium\n3. Large")
                while True:
                    size = input("Choose what size you would like by entering the number: ").strip().lower()
                    try:
                        if size == "1":
                            while True:
                                size_confirmation = input("\nWould you like to add a Small Tropical drink to your order? (Yes or No): ").strip().lower()
                                try:
                                    if size_confirmation == "yes":
                                        drinks.append("- Small Tropical")
                                        return
                                    elif size_confirmation == "no":
                                        drink_selection()
                                    else:
                                        raise InvalidConfirmation
                                except InvalidConfirmation:
                                    print("Please input a valid answer (Either 'Yes' or 'No').")
                        elif size == "2":
                            while True:
                                size_confirmation = input("\nWould you like to add a Medium Tropical drink to your order? (Yes or No): ").strip().lower()
                                try:
                                    if size_confirmation == "yes":
                                        drinks.append("- Medium Tropical")
                                        return
                                    elif size_confirmation == "no":
                                        drink_selection()
                                    else:
                                        raise InvalidConfirmation
                                except InvalidConfirmation:
                                    print("Please input a valid answer (Either 'Yes' or 'No').")
                        elif size == "3":
                            while True:
                                size_confirmation = input("\nWould you like to add a Large Tropical drink to your order? (Yes or No): ").strip().lower()
                                try:
                                    if size_confirmation == "yes":
                                        drinks.append("- Large Tropical")
                                        return
                                    elif size_confirmation == "no":
                                        drink_selection()
                                    else:
                                        raise InvalidConfirmation
                                except InvalidConfirmation:
                                    print("Please input a valid answer (Either 'Yes' or 'No')")
                        else:
                            raise InvalidSize
                    except InvalidSize:
                        print("\nPlease input a valid number (1 - 3).")
            else:
                raise InvalidDrinkSelection
            break
        except InvalidDrinkSelection:
            print("\nPlease input a valid number (1 - 4).") 

drink_selection()
for i in range(0, len(drinks)):
    print("Your order:\n{}".format(drinks[i]))

