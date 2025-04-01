# plp-python-week3
Create a function named calculate_discount(price, discount_percent) that calculates the final price after applying a discount. The function should take the original price (price) and the discount percentage (discount_percent) as parameters. If the discount is 20% or higher, apply the discount; otherwise, return the original price.
Using the calculate_discount function, prompt the user to enter the original price of an item and the discount percentage. Print the final price after applying the discount, or if no discount was applied, print the original price..
#Create a function named calculate_discount(price, discount_percent)

def calculate_discount(price, discount_percent):
    if discount_percent >= 20:
        discount_amount = price * (discount_percent / 100)
        final_price = price - discount_amount
        return final_price
    else:
        return price
    
input_price = float(input("Enter the original price of the item: "))
input_discount = float(input("Enter the discount percentage: "))

print("Final price after applying discount: $", calculate_discount(input_price, input_discount))
