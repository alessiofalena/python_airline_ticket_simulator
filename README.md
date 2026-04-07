# Python Airline Ticket Booking Simulator

A Python simulation of an airline ticket management system, modelled on the real purchase flow of Ryanair's website. Built as a practical project during the Python module of the Data Analysis course at Start2Impact.

## Project Overview

The system allows users to register, generate, view, search, and analyse airline tickets, replicating the variables and logic of a real booking process, including ticket types, seat selection, baggage options, and extra services.

## Functions

### `register_new_ticket()`
Interactively registers a new ticket through user input. Handles:
- Passenger name and purchase timestamp
- Ticket type selection: Basic, Regular, Plus, Flexiplus
- Seat selection (manual or random, depending on ticket type)
- Extra services: Fast Track, Priority Boarding, 10kg cabin bag
- Baggage options: 10kg and 20kg check-in bags (with type-specific rules)
- Duplicate detection and input validation via `while` loops

### `generate_multiple_random_tickets(n)`
Generates `n` random tickets automatically using the `random` library — useful for populating the system with test data.

### `show_registered_tickets()`
Displays all registered tickets with their full attributes in a readable format.

### `search_ticket_interactive()`
Allows the user to search for tickets by a single attribute (e.g. Ticket Type, Passenger Name, Reserved Seat). Displays all possible values for the chosen attribute before prompting for input.

### `show_ticket_statistics()`
Displays a summary of the registered tickets, including:
- Total ticket count
- Percentage distribution by ticket type
- Min, max, and average baggage counts (10kg and 20kg)
- Fast Track and Priority Boarding totals
- Tickets sold in the last 30 days
- Last ticket registered

### `search_ticket_by_multiple_attributes()`
Advanced search: allows filtering tickets by multiple attribute-value pairs simultaneously. Iterates through all tickets and returns only those matching all specified conditions.

## Technologies

- **Python 3**
- **Jupyter Notebook**
- Standard libraries: `datetime`, `random`, `collections`

## Python Concepts Used

- Functions with parameters and docstrings
- Dictionaries and lists
- `while` loops for input validation
- `for` loops and `enumerate`
- `Counter` from `collections`
- f-strings and string manipulation
- Conditional logic (`if/elif/else`)
- `datetime` and `timedelta` for time-based filtering

## Repository Structure

```
python_airline_ticket_simulator/
│
├── AlessioFalena_Python.ipynb   # Full project notebook
└── README.md                    # Project overview
```

## Author

**Alessio Falena**  
[LinkedIn](https://www.linkedin.com/in/alessiofalena/) | [GitHub](https://github.com/alessiofalena)