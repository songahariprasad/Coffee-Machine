# Coffee Machine

This project is a simple coffee machine program written in Python. The coffee machine can serve three types of coffee: espresso, latte, and cappuccino. It handles resources like water, milk, and coffee, and processes payments using coins.

## Features

- **Menu Options**: Choose from espresso, latte, and cappuccino.
- **Resource Management**: Tracks the resources (water, milk, coffee) required to make coffee.
- **Payment Processing**: Calculates the total amount of money inserted and determines if it is sufficient for the chosen drink.
- **Transaction Handling**: Manages successful transactions and provides change if necessary.
- **Reporting**: Displays the current resources and profit.
- **Exit Option**: Turn off the machine by typing "off".

## Getting Started

### Prerequisites

- Python 3.x installed on your machine.

### Running the Program

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/coffeemachine.git
    ```

2. Navigate to the project directory:
    ```sh
    cd coffeemachine
    ```

3. Run the program:
    ```sh
    python coffeemachine.py
    ```

### Usage

- When prompted, enter your choice of coffee (`espresso`, `latte`, `cappuccino`).
- If you want to check the resources and profit, type `report`.
- To turn off the machine, type `off`.

### Example

- What would you like? (espresso/latte/cappuccino): latte
- Please insert coins.
- how many 10's?: 2
- how many 20's?: 1
- how many 50's?: 0
- how many 100's?: 0
- Here is $0.0 in change.
- Here is your latte ☕️. Enjoy!


## Code Structure

- **MENU**: Dictionary containing the available drinks, their ingredients, and cost.
- **resources**: Dictionary tracking the available amounts of water, milk, and coffee.
- **is_resource_sufficient(order_ingredients)**: Checks if there are enough resources to make the selected drink.
- **process_coins()**: Handles coin input and calculates the total amount of money inserted.
- **is_transaction_successful(money_received, drink_cost)**: Determines if the inserted money is sufficient for the drink and processes the transaction.
- **make_coffee(drink_name, order_ingredients)**: Deducts the used ingredients from the resources and serves the drink.
