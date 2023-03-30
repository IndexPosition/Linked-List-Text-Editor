# Linked List Text Editor - Capstone Project

## Overview

This project is a simple text editor that uses a double linked list to store text. It allows the user to perform basic text editing operations such as inserting and deleting text, as well as undoing and redoing previous changes. It also uses the concept of Stack.

## Technologies Used

- HTML
- CSS
- JavaScript

## Features

- Undo and redo functionality using linked list
- Clear text area
- Save and open files

## How to Use

To use the text editor, simply open the `index.html` file in a web browser or [Click Here](). The text editor interface will open, allowing you to type and edit text.
You can start typing in the text area, and use the following buttons to manage the input:

1. Undo: Undo the last change made to the text area.
2. Redo: Redo the last change undoed.
3. Clear: Clear the text area (memory) and start over.
4. Save: Save the current text to a file with a specified name.
5. Open: Open a previously saved file and load its contents into the text area.

## How it Works

This text editor uses doubly linked list data structure to store the text. Each node in the linked list represents a single character in the text, and contains a reference to the next and previous nodes.

The text editor keeps track of the current node in the linked list, which represents the cursor position. When the user types a character, a new node is inserted after the current node, and the current node is updated to point to the new node. When the user deletes a character, the current node is simply updated to point to the previous node.

The text editor also keeps track of the user's editing history using a stack. When the user performs an editing operation, such as inserting or deleting a character, the current state of the linked list is pushed onto the stack. If the user wants to undo the last operation, the previous state of the linked list is popped from the stack and restored.

## Acknowledgments

- https://www.geeksforgeeks.org/data-structures/linked-list/
- https://www.geeksforgeeks.org/implementation-linkedlist-javascript/
- https://www.tutorialspoint.com/how-to-create-and-save-text-file-in-javascript
