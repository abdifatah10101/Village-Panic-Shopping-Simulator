# Village Panic Shopping Simulator

A Python mini-adventure project demonstrating store management, inventory tracking, input validation, and simple game logic. Developed step-by-step through Versions 1.0 to 1.5 and Version 2.0.

## Overview

Your village is under attack, and you must run through three shops to collect supplies before trouble arrives. Each store has its own list of items and prices. You can buy items, skip stores, avoid invalid choices, manage your gold, and watch how the full inventory changes over the course of the day. At the end, a combined "department store" inventory is printed for both morning and evening, showing exactly what was purchased.

This project demonstrates practical use of loops, dictionary manipulation, conditional logic, user input handling, and multi-version program development.

---

# Features by Version

## Version 1.0 – Basic Store System

* Player visits each store.
* Store items are listed.
* Player types an item name to buy it.
* Purchased items are saved in the cart dictionary.
* Items purchased are removed from store inventories.

## Version 1.1 – Skipping Stores

* Player may type "exit" to skip a store.
* Program moves on to the next store without a purchase.

## Version 1.2 – Invalid Input Handling

* If the player enters an item not found in the store, the program prints "Invalid choice" and continues.

## Version 1.3 – Tracking All Choices

* All player choices, including "exit", are stored.
* If the player types "exit" for all three stores, the program prints a message that nothing was purchased.

## Version 1.4 – Gold and Pricing System

* Player begins with 1000 gold.
* All items have prices assigned in the store dictionaries.
* When a purchase is made:

  * The price is retrieved.
  * Total spending increases.
  * The player's gold is reduced.
  * The purchased item is removed from the store inventory.
* At the end, the program displays:

  * The items purchased
  * Total cost
  * Remaining gold

## Version 1.5 – Morning and Evening Inventory Merge

Big Biz requires full inventory reports.

Two combined inventories are created:

1. Morning inventory: before any purchases
2. Evening inventory: after all purchases

Process:

* A new dictionary is created.
* Each store is looped over.
* The "name" field is skipped.
* Only real items are added with their prices.
* Final inventory lists are printed in sorted order.

These lists show exactly what was available at the start and what remained at the end.

---

# Program Flow Summary

1. Build morning combined inventory.
2. Loop through each store and print its available items.
3. Player chooses an item or types "exit".
4. Handle invalid input.
5. For valid purchases:

   * Update gold
   * Update total spending
   * Add item to cart
   * Remove the item from the store
6. After all stores:

   * If all choices were "exit", print a no-purchase message.
   * Otherwise, print purchase summary.
7. Build the evening combined inventory.
8. Print morning and evening inventories for comparison.

---

# Concepts Demonstrated

* Dictionary creation, updating, and popping
* Looping through nested data structures
* User input handling and validation
* Tracking game state across multiple iterations
* Calculating totals and updating values
* Filtering keys (skipping "name")
* Merging multiple dictionaries
* Sorted output formatting
* Multi-step versioned development
