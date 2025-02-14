# Decode Secret Message

This project is a fun and creative solution to a code puzzle where the goal is to decode a hidden message from a set of grid-based coordinates and character data. The script reads input data containing coordinates and characters, builds a grid from this information, and reveals the secret message by aligning the characters according to their specified positions.


## Table of Contents
- [How It Works](#how-it-works)
- [Usage](#usage)
- [Changing the Input Data](#changing-the-input-data)
- [Project Files](#project-files)
- [Fun Tips](#fun-tips)
- [Motivation](#motivation)
- [Contribution](#contribution)
- [License](#license)

 
## How It Works
The code performs the following steps:
1. **Data Parsing:**
   - Reads input data containing rows formatted as `x-coordinate character y-coordinate`.
   - Extracts the coordinates and associated characters.

2. **Grid Construction:**
   - Builds a grid of characters by placing each character at its corresponding coordinate.
   - Fills empty spaces with blank characters for better visualization.

3. **Message Decoding:**
   - Outputs the constructed grid to reveal the hidden message.

## Example Input
Here is an example snippet of input data:
```plaintext
93 ░ 5
2 ░ 5
8 ░ 0
39 █ 1
...
```

## Sample Output
If the input contains coordinates that form a recognizable pattern, the script prints something like:
```plaintext
████░░
░░███░
██░░██
```
The exact output depends on the input data provided.

## For the given data the output will look like this:
<img src="https://github.com/roshaanmehar/Secret-Message-Decoder/blob/main/Screenshot%202025-02-08%20232536.png" width="500">
## Usage
To run the script, simply execute it with Python:
```bash
python decode_message.py
```

### Changing the Input Data
Replace the `data` variable in the script with your own set of coordinate-character data to decode other messages. You can also use AI to generate sample data.

## Project Files
- **decode_secret_message.py:** The main script containing the logic for decoding the secret message.

## Fun Tips
- Experiment with different input patterns to create artistic outputs.
- Try using various characters for more creative grid visuals.
- Share your coolest grid-based messages!

## Motivation
This script was created as a fun coding challenge and puzzle-solving exercise. It's a great example of how simple coordinate mapping can uncover complex visual patterns.

## Contributing
Found a cool pattern or have suggestions to enhance the grid visualization? Feel free to contribute or share your ideas!

## License
This project is for fun and educational purposes and does not require any formal licensing.

