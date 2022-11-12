# Week 7 Lab Report

### Changing the name of the "start" parameter and its uses to "base" 

Sequence of characters pressed:     
`vim DocDocSearchServer.java<enter></>start<enter><c><e>base<esc><n><.><n><.><n><.><:><w><q>`

Description:   
1. Type vim DocSearchServer.java to edit this file
2. Press `<enter>` to run command
3. Press `</>` then type **"start”** to find the first instance of start from the location of the cursor
4. Press `<enter>` to run the command and search for the word **"start"**. This places the cursor at the location of "**s**" in **"start"**.
5. Press `<c>` to prompt change command at the location of the cursor.
6. Press `<e>` to prompt end command. This lets terminal knows you are changing the whole word.
7. Type **"base"**. This replaces the word "**start**" with the word "**base**".
8. Press `<esc>` to get back to normal mode
9. Press `<n>` to find the next instance of start 
10. Press `<.>` to automatically repeat steps 5 and 6.
11. We repeated step 9 and 10 until we find and replace all the variables "**start**" with "**base**".    
12. Press `<:><w><q>` sequentially to save changes and exit.   `<w>` stands for write and `<q>` stands for quit.


