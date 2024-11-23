print("Welcome to the tip calculator")

bill = float(input("What is your total bill? $"))

tip = int(input("What percentage tip would you like to give? 10 15 20 25: "))

people = int(input("How many people split the bill? "))

sales_tax = {
    "alabama": 0.04, "alaska": 0.0, "arizona": 0.056, "arkansas": 0.065, "california": 0.0725, 
    "colorado": 0.029, "connecticut": 0.0635, "delaware": 0.0, "florida": 0.06, "georgia": 0.04, 
    "hawaii": 0.04, "idaho": 0.06, "illinois": 0.0625, "indiana": 0.07, "iowa": 0.06, 
    "kansas": 0.065, "kentucky": 0.06, "louisiana": 0.0445, "maine": 0.055, "maryland": 0.06, 
    "massachusetts": 0.0625, "michigan": 0.06, "minnesota": 0.06875, "mississippi": 0.07, "missouri": 0.04225, 
    "montana": 0.0, "nebraska": 0.057, "nevada": 0.0685, "new hampshire": 0.0, "new jersey": 0.06625, 
    "new mexico": 0.05125, "new york": 0.04, "north carolina": 0.0475, "north dakota": 0.05, "ohio": 0.0575, 
    "oklahoma": 0.045, "oregon": 0.0, "pennsylvania": 0.06, "rhode island": 0.07, "south carolina": 0.06, 
    "south dakota": 0.04, "tennessee": 0.07, "texas": 0.0625, "utah": 0.0685, "vermont": 0.06, 
    "virginia": 0.053, "washington": 0.065, "west virginia": 0.06, "wisconsin": 0.05, "wyoming": 0.04
}

print("Please choose your state from the following list:")
for state in sales_tax:
    print(state.title())

while True:
    state = input("Which state are you in? ").lower()

    if state in sales_tax:
        tax_rate = sales_tax[state]  
        break 
    else:
        print(f"Sorry, sales tax information not available for {state.title()}. Please try again.")

total_tax_amount = bill * tax_rate  
tip_as_percentage = tip / 100
total_tip_amount = bill * tip_as_percentage
total_bill_amount = bill + total_tax_amount + total_tip_amount
bill_per_person = total_bill_amount / people
final_amount = round(bill_per_person, 2)
print(f"Each person should pay: ${final_amount}")
