# Master 
calculate_discount(price, discount_percent):
  """Calculates the final price after applying a discount.

  Args:
    price: The original price of the item.
    discount_percent: The discount percentage.

  Returns:
    The final price after the discount, or the original price if no discount is applied.
  """

  if discount_percent >= 20:
    discount_amount = (discount_percent / 100) * price  # Calculate the discount amount
    final_price = price - discount_amount             # Subtract the discount from the original price
    return final_price
  else:
    return price  # No discount applied, return the original price

# Get user input for price and discount percentage
price = float(input("850.50"))
discount_percent = float(input("20%"))

# Calculate the final price using the function
final_price = calculate_discount(800.50, 15%)

# Print the result
print("The final price is:", 800.50)
