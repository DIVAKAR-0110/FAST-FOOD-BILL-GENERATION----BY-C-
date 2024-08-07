# Billing System for Food Shops
## Overview

This project is a billing system for food shops, designed to help manage and generate bills for customers. The system allows users to input menu items, take orders, calculate totals with applicable taxes, and display or save the bill.
## Features

    Add menu items with prices.
    Display a menu card for the day.
    Take customer orders and quantities.
    Calculate the subtotal, SGST, and CGST.
    Display and save the bill with all details.
    Option to reset quantities and generate new bills.

## Requirements

    C++ compiler
    Standard C++ library

##Usage

    Compile the code:

    bash

g++ -o billing_system billing_system.cpp

# Run the executable:

bash

    ./billing_system

    Follow the prompts:
        Enter the number of items.
        Input the name and price for each item.
        Select items and their quantities for the order.
        Generate and display/save the bill.

# Code Overview
## Main Classes and Functions

    FoodItem Class
        Encapsulates details of each menu item (name, price, quantity).

    FoodShop Class
        Manages the operations of the shop including adding items, displaying the menu, taking orders, displaying bills, and resetting quantities.

## Key Functions

    void addItem(string name, int price);
        Adds a new item to the menu.
    void displayMenu() const;
        Displays the current menu.
    void takeOrder();
        Takes orders from customers.
    void displayBill(ofstream &obj) const;
        Displays and saves the bill to a file.
    void resetQuantities();
        Resets quantities for a new order.

#Constants

    const double SGST_RATE = 0.06;
    const double CGST_RATE = 0.06;
