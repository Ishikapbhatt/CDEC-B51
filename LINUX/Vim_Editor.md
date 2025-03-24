**# Mastering Text Editing with VIM**

**Modes:**

**Normal Mode:** Default mode where you can navigate, delete, copy, paste, and perform other actions without typing the content.

**Insert Mode:** Where you actually type your content (like any other text editor).

**Visual Mode:** Used for selecting text (like highlighting in other text editors).

**Command Mode:** Used to enter commands to save, quit, search, etc.

**Basic Movement:** In Normal Mode, you can use the following keys to move the cursor around:

**h -** left

**j**- down

**k -** up

**l -** right

**Editing:**

**Press i** to switch to Insert Mode to start typing.

**Press Esc** to return to Normal Mode.

**Saving and Quitting:**

**To save:** :w

T**o quit:** :q

**To save and quit:** :wq

**To quit without saving:** :q!

![image](https://github.com/user-attachments/assets/04a657ca-b4c3-4054-aa8d-12241dfa211f)

![image](https://github.com/user-attachments/assets/ff16bcd4-b265-4652-a0ff-03cb865c511f)

![image](https://github.com/user-attachments/assets/3af0be06-a668-4dad-91de-9d260c480ab1)


**To delete the word move the cursor to the beginning of the word and use dw command in normal mode. The word under the cursor will be deleted.**

dw

**To delete more than one word in a single line use the following command.**

**To delete 2 words use the command**

d2w

**To delete the line move cursor to the beginning of the line and use d$ command in normal mode. The line under the cursor will be deleted.**

d$

**Undo and Redo:**

**As we are programmers most time we are using undo and redo .vim to provide these to both features in it. To undo press u key in normal mode**

u

**To redo use the ctrl+r key in normal mode in vim**

ctrl+r

**Search in Vim Editor**

**To search the word After the cursor uses the backslash key and then write the word and press enter.**

:/word

**Use n to move on next matching word**

:n

**Use N to move on previous matching word**

:N

**Search and Replace in Vim Editor**

**To replace the word in file use s/ command in vim like**

:s/searchword/replaceword/

**To do replace all occurrence of word use g**

:s/searchword/replaceword/g

**This command will replace the word globally.**

**To confirm before replacements of words use gc.**

:s/searchword/replaceword/gc

**To use this command in the whole file use % before the command.**

:%s/searchword/replaceword/gc
