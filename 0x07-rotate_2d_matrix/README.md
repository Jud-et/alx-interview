📦 0x07 - Rotate 2D Matrix
Welcome to the world of matrix magic! 🎩✨ In this project, we’re going to rotate a 2D matrix by 90 degrees clockwise using a snazzy in-place algorithm. No fancy tools, no extra space – just pure matrix manipulation awesomeness.

🚀 Overview
We’ve got ourselves an n x n 2D matrix, and our mission is to rotate it 90° clockwise. Think of it as a cool twist for your data! 🌀

Input: A 2D matrix (guaranteed to be non-empty and square, because we like to keep things neat).
Output: None. We're changing the matrix in-place, so no new matrix allowed – you edit the existing one right there!
✨ Matrix Rotation - The Game Plan
Here’s how we pull off this 90-degree spin:

Transpose the Matrix – Basically swapping rows and columns (fancy way to say “turn things sideways”).
Reverse Each Row – Flip those rows like pancakes, and bam, we’ve got a 90-degree rotation! 🥞:
Watch the magic unfold as your matrix rotates like a pro! 🎉

📜 Function Prototype
Here’s what your matrix-rotating hero looks like:

python
Copy code
def rotate_2d_matrix(matrix):
    """
    Rotate the matrix in-place by 90 degrees clockwise.
    """
🧠 Concepts You’ll Need
To tackle this, you'll need to sharpen your skills in the following areas:

Matrix Representation – Lists of lists in Python, baby!
In-place Operations – Why create new matrices when we can save space by modifying the original?
Transposition – Swap rows and columns like it’s no big deal.
Reversing Rows – Flip ‘em like pancakes and voilà – rotation achieved.
📝 Requirements
All files will be interpreted/compiled on Ubuntu 20.04 LTS using Python3 (version 3.8.10).
Your code should follow pycodestyle (version 2.8.0) standards – because clean code is happy code!
You are not allowed to import any modules – we’re doing this old-school.
📚 Resources
If you need some extra reading, check out:

Python Lists – Tutorialspoint
In-place Rotate Matrix – GeeksforGeeks
Matrix Transpose – Single Line Solution
