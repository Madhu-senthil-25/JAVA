# GROCERYAPP
import java.util.Scanner;

// Class representing a grocery item
class GroceryItem {
    String itemName;
    double price;

    // Method to set item details using user input
    void setItemDetails(String name, double cost) {
        itemName = name;
        price = cost;
    }

    // Method to display item info
    void displayItem() {
        System.out.println("Item Name: " + itemName);
        System.out.println("Price:" + price);
    }
}

// Main class
public class GroceryApp {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        GroceryItem item = new GroceryItem();

        // Take user input
        System.out.print("Enter item name: ");
        String name = input.nextLine();

        System.out.print("Enter item price: ");
        double price = input.nextDouble();

        // Set and display item
        item.setItemDetails(name, price);
        item.displayItem();

        input.close(); // Close the scanner
    }
}
