Secret Message Decoder

This repository contains a fun piece of code that reads a list of (x, character, y) values and reconstructs a visual grid of those characters, effectively revealing a hidden or “secret” message. It was created as a puzzle-solving exercise and can be extended for various coordinate-based code-breaking problems.
How It Works

    Input Format
    The code expects a string of lines. Each line has three parts:
        An integer x (the x-coordinate),
        A single character char (like █ or ░ or any other symbol),
        An integer y (the y-coordinate).

    Example input (one line):

    93 ░ 5

    This means the character ░ should appear at coordinates (x=93, y=5) in the grid.

    Parsing
    The function decode_secret_message(data):
        Splits the input string into lines.
        For each line, it extracts x, char, and y.
        Stores these in a dictionary called grid, using (x, y) as the key and char as the value.
        Also keeps track of the maximum x and y seen, so it knows how big the grid needs to be.

    Reconstructing the Grid
    Once all (x, y) -> char mappings are stored:
        It loops through each row from y=0 to y=max_y.
        For each row y, it builds a string from x=0 to x=max_x, filling in the character from grid[(x, y)] if it exists, or a space ' ' if it doesn’t.
        Stores each row in result_grid for final printing.

    Output
    Prints the final grid line by line. If your data positions the characters in a specific pattern, you’ll see the puzzle or hidden image revealed in the console.

Usage

    Clone or Copy this repository/code snippet.
    Install Python (version 3.x).
    Run the script:

    python decode_secret_message.py

    Or simply place the function in a script or notebook and execute it with the desired input string.
    Inspect the Output in the console. You’ll see the ASCII-art or symbol-based secret message.

Example

Given a snippet of data like:

93 ░ 5
2 ░ 5
8 ░ 0
...

the code prints out a visually coherent message or pattern (for instance, ASCII art, partial images, or words spelled out using █ and ░ characters).
Customizing

    Change Characters: You can replace the █ and ░ with any symbols you like.
    Grid Orientation: Currently, rows increase with y. If you want to invert the vertical orientation, you could iterate from max_y down to 0.
    Data Source: You can pull data from a file or network source. Just parse that data into the same format the function expects.

Contributing

This was just a fun, quick project. If you’d like to expand its functionality—e.g., add color, handle multi-character tokens, or invert the axes—feel free to fork and submit a pull request!
