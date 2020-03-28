# Automathon

Automation Anywhwere software used to create Bots which does the following activities along with salient features are listed with their description details
Download the encrypted file, decrypt it and open

This bot will download the attachment from the email, decrypt it and then open the file
Logic

    The credentials are stored in local excel sheet, so retrieving the username and password and storing them in the local variables
    Looping through all the email and downloading all the attachment
    If the desired email subject is obtained exiting the loop
    Copying only the desired attachment
    Deleting all the other irrelavent attachmment from the download folder
    Decrypting the file using the same key used for encrypting
    Opening the decrypted file

Extract PDF data to Excel, encypt it then send via email

This Bot is to extract the data from the PDF and those fields will be saved in the excel. This excel is then encryptrd and send via email
Logic

    The credentials are stored in local excel sheet, so retrieving the username and password and storing them in the local variables
    Extracting the data from the PDF and storing those fields in the variables
    Opening the excel sheet and entering the extracted fields in the excel cells
    Encrypting the excel file after closing it
    Sending to user via email

Deletion of empty rows

There are many cases where the Key will be empty in the excel sheet, this bot is designed to delete those rows.

Approach: Down to top Why: If we delete the rows from top to bottom, there is a chance of infinite loop as well as if we delete a row, the total number of rows which has data will change, thus loop will not be correct

Explanation:

    Program will prompt for the file path, if we choose yes, it will proceed with default excel. If we want to give a excel path, choose No and provide the path
    Bot will open the excel and if not able to find the excel it throw the warning message
    Bot will check whether any of the row is empty using the down to top loop, if found it will delete the row
    Closes the excel sheet


