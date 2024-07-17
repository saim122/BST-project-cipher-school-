Binary Search Tree (BST) Implementation in Java
This repository contains an implementation of a Binary Search Tree (BST) in Java, featuring essential functionalities including insertion, search, and deletion operations.

Features
Insertion: Add nodes to the BST while maintaining the BST property.
Search: Locate nodes within the BST.
Deletion: Remove nodes from the BST, handling all cases (node with no children, one child, and two children).
Classes
TreeNode
Represents a node in the BST.

Fields:
int val: The value of the node.
TreeNode left: The left child node.
TreeNode right: The right child node.
Constructor: Initializes the node with a given value and sets left and right children to null.
BST
Handles the operations on the BST.

Methods:
void insert(int key): Inserts a node with the specified key.
TreeNode search(int key): Searches for a node with the specified key.
void delete(int key): Deletes a node with the specified key.
TreeNode minValue(TreeNode root): Helper method to find the node with the minimum value in a given subtree.

public class Main {
    public static void main(String[] args) {
        BST tree = new BST();

        // Insert elements
        tree.insert(50);
        tree.insert(30);
        tree.insert(20);
        tree.insert(40);
        tree.insert(70);
        tree.insert(60);
        tree.insert(80);

        // Search for a value
        TreeNode result = tree.search(40);
        System.out.println(result != null ? "Found: " + result.val : "Not found");

        // Delete elements
        tree.delete(20);
        tree.delete(30);
        tree.delete(50);
    }
}
Project Structure
TreeNode.java: Defines the structure of a tree node.
BST.java: Contains the BST implementation with insert, search, and delete methods.
Main.java: Demonstrates the usage of the BST class.

Getting Started
Clone the repository.
Open the project in your preferred Java IDE.
Run Main.java to see the BST in action.
Contributions
Feel free to fork this repository, submit issues, and send pull requests. Any contributions to improve the functionality and efficiency of this BST implementation are welcome.
