# Answers

Task 1

Answer the questions below

Install Vim

No answer needed

Launch Vim

No answer needed

**************

Task 2

Answer the questions below

How do we enter "INSERT" mode?

i

How do we start entering text into our new Vim document?

typing

How do we return to command mode?

esc

How do we move the cursor left?

h

How do we move the cursor right?

l

How do we move the cursor up?

k

How do we move the cursor down?

j

How do we jump to the start of a word?

w

How do we jump to the end of a word?

e

How do we insert (before the cursor)

i

How do we insert (at the beginning of the line?)

I (capital i)

How do we append (after the cursor)

a

How do we append (at the end of the line)

A

How do we make a new line under the current line?

o

******** 

Task 3

Answer the questions below

How do we write the file, but don't exit?

```bash
:w
```

How do we write the file, but don't exit- as root?

```bash
:w !sudo tee %
```

How do we write and quit?

```bash
:wq
```

How do we quit?

```bash
:q
```

How do we force quit?

```bash
:q!
```

How do we save and quit, for all active tabs?

```bash
:wqa
```

******** 

Task 4

Answer the questions below

How do we copy a line?

Submit

To copy a line in Vim, you can use the `yy` command. This command yanks (copies) the current line, allowing you to paste it elsewhere in the file. Here's how to do it:

1. **Ensure You Are in Normal Mode:**
If you are not sure, press `Esc` to switch to normal mode.
2. **Copy the Line:**
Type `yy` (short for yank line) and press `Enter`.

This command copies the entire current line.

### Example Workflow

Suppose you have the following lines in your file:

```
Line 1
Line 2
Line 3

```

1. **Open the file in Vim:**
    
    ```
    vim example.txt
    
    ```
    
2. **Ensure You Are in Normal Mode:**
    - Press `Esc` to ensure you are in normal mode.
3. **Copy a Line:**
    - Position the cursor on the line you want to copy (e.g., "Line 2").
    - Type `yy` and press `Enter`.

The line "Line 2" is now copied and ready to be pasted.

To paste the copied line, move the cursor to the desired location and use the `p` command to paste after the cursor or `P` to paste before the cursor. For example:

- To paste after the cursor: Type `p` and press `Enter`.
- To paste before the cursor: Type `P` and press `Enter`.

how do we copy 2 lines?

Submit

To copy two lines in Vim, you can use the following steps:

1. **Ensure You Are in Normal Mode:**
If you are not sure, press `Esc` to switch to normal mode.
2. **Navigate to the Starting Line:**
Move the cursor to the first line you want to copy.
3. **Enter Visual Line Mode:**
    - Press `Shift + V` to enter visual line mode. This mode allows you to select entire lines.
4. **Select the Lines:**
    - Move the cursor down to the second line you want to copy. This will highlight both lines.
5. **Copy the Lines:**
    - Press `y` (yank) to copy the selected lines.

The selected lines are now copied and can be pasted elsewhere in the file using the `p` command (paste).

### Example Workflow

Suppose you want to copy lines 3 and 4 in the following text:

```
1. First line
2. Second line
3. Line to copy 1
4. Line to copy 2
5. Fifth line

```

1. **Open the File in Vim:**
    
    ```
    vim example.txt
    
    ```
    
2. **Ensure You Are in Normal Mode:**
    - Press `Esc` to ensure you are in normal mode.
3. **Navigate to the Starting Line:**
    - Move the cursor to line 3 ("Line to copy 1").
4. **Enter Visual Line Mode and Select Lines:**
    - Press `Shift + V` to enter visual line mode.
    - Move the cursor down to line 4 ("Line to copy 2"). Both lines should now be highlighted.
5. **Copy the Lines:**
    - Press `y` to copy the selected lines.

Now you can paste these lines elsewhere in the file using the `p` command.

To copy two lines in Vim, you can use the following steps:

1. **Ensure You Are in Normal Mode:**
If you are not sure, press `Esc` to switch to normal mode.
2. **Navigate to the Starting Line:**
Move the cursor to the first line you want to copy.
3. **Enter Visual Line Mode:**
    - Press `Shift + V` to enter visual line mode. This mode allows you to select entire lines.
4. **Select the Lines:**
    - Move the cursor down to the second line you want to copy. This will highlight both lines.
5. **Copy the Lines:**
    - Press `y` (yank) to copy the selected lines.

The selected lines are now copied and can be pasted elsewhere in the file using the `p` command (paste).

### Example Workflow

Suppose you want to copy lines 3 and 4 in the following text:

```
1. First line
2. Second line
3. Line to copy 1
4. Line to copy 2
5. Fifth line

```

1. **Open the File in Vim:**
    
    ```
    vim example.txt
    
    ```
    
2. **Ensure You Are in Normal Mode:**
    - Press `Esc` to ensure you are in normal mode.
3. **Navigate to the Starting Line:**
    - Move the cursor to line 3 ("Line to copy 1").
4. **Enter Visual Line Mode and Select Lines:**
    - Press `Shift + V` to enter visual line mode.
    - Move the cursor down to line 4 ("Line to copy 2"). Both lines should now be highlighted.
5. **Copy the Lines:**
    - Press `y` to copy the selected lines.

Now you can paste these lines elsewhere in the file using the `p` command.

How do we copy to the end of the line?

y$

How do we paste the clipboard contents after the cursor?

p

How do we paste the clipboard contents before the cursor?

P

How do we cut a line?

dd

How do we cut two lines?

2dd

How do we cut to the end of the line?

D

How do we cut a character?

x

******** 

Task 5

Answer the questions below

How do we search forwards for a pattern (use "pattern" for your answer)

```bash
#Vim will move the cursor to the first occurrence of "example". To find the next occurrence, press n.
/pattern
```

How do we search backwards for a pattern (use "pattern" for your answer)

?pattern

How do we repeat this search in the same direction?

n

How do we repeat this search in the opposite direction?

N

How do we search for "old" and replace it with "new"

```bash
:%s/old/new/g
```

How do we use "grep" to search for a pattern in multiple files?

***vimgrep (so you have to add word after this like “ :vimgrep hello”)***
