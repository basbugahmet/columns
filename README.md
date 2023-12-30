
# **Columns Game**

The aim of this project is to develop a numerical game titled "Columns."

**1. Game Initialization:**

-   Initialize 5 columns and a box with numbers 1-10.
-   Shuffle and distribute 50 numbers among the columns, ensuring each column has 6 numbers.

**2. Game Operations:**

-   Two operations: Column to column number transferring and drawing a number from the box.

**3. Column to Column Number Transferring:**

-   Select a number from a column using the Z key.
-   Select another column using the X key for transferring.
-   Transferred numbers are appended to the destination column under specific conditions.

**4. Drawing a Number from the Box (Then Transferring):**

-   Draw a number from the box using the B key.
-   Select a column using the X key for transferring.
-   The drawn number is transferred to the end of the selected column under specific conditions.

**5. Transfer Conditions:**

-   Difference between the selected number (from-column or drawn) and the last number in the to-column must be 0, 1, or -1.
-   If the to-column is empty, the top number of the transferred numbers must be 1 or 10.

**6. Scoring:**

-   Aim to form an ordered set (1-2-3-4-5-6-7-8-9-10) or reverse ordered set (10-9-8-7-6-5-4-3-2-1) in a column.
-   Player receives 1000 points for each completed ordered set, and the set disappears.
-   End game score calculated by the formula: `End-Game Score = 100 * Finished Ordered Sets + (Score / Transfer Number)`

**7. End of the Game:**

-   Player can finish the game by collecting 5 ordered sets or exit by pressing E key.

**8. High Score Table:**

-   Display High Score Table for end-game scores in descending order.
-   Default High Score Table in "highscore.txt" file.

**9. Data Structures:**

-   Box: Singly Linked List (SLL).
-   High Score Table: Doubly Linked List (DLL).
-   Columns: Multi Linked List (MLL).
