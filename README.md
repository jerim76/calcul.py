# calcul.pydef calculate_discount(price, discount_percent):
    """Calculates the final price after applying a discount if it's 20% or higher."""
    if discount_percent >= 20:
        final_price = price - (price * discount_percent / 100)
        return final_price
    return price  # Return original price if discount is less than 20%

# Get user input
price = float(input("Enter the original price: "))
discount_percent = float(input("Enter the discount percentage: "))

# Calculate and display the final price
final_price = calculate_discount(price, discount_percent)
print(f"The final price is: {final_price:.2f}")

