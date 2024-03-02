# myPhone
Learnable task 8

Lets start with the basics, this is a console application json file linked as a database for my contact list and a call history. 
RUN node phone.js to start

##### Test Numbers:
- Contact: RedX - 09065795264
- Unsaved number - 07011000011

## Phone Class
My main class constructor with multiple methods included. I build my code by asking what I'd expect to see on the real thing so I included the following:
- Phone numbers
- Contacts loaded from contacts.json with its own methods for saved contacts (Add, Edit, Delete and dial.)
- A call history
- A dialing function for unsaved phone numbers.
- A regex to maKe sure these are real phone numbers.
- for creating and accessing, editing amd saving data like the call_history.json file which stores the phone number and a timestamp for the dialed number.

- it also includes codes for accessing the contacts list in the file, contacts.json, 

## Contacts
I built the contacts object and included several methods of the phone class to provide the following functionalities:
-- add contact
-- edit contact
-- remove/delete contact 
-- dial contact
All these methods have notifiers for each action

### Observers
 Includes an observer object with two observer classes, observer1 and observer2 with methods for adding, removing and notifying observers with notifications for different actions, not just dialing. 
 Why I did this? it just didn't make sense to leave the others out. Chalk it up to equality.
- ###### Yeah...I got rid of most of that. Too much clutter.

### The interface:

The interface offers a menu with responses to be provided as numbers.  
Attempting to dial a phone number absent from the contacts list returns an error message. Maybe making it console.error would be best. Console.log works just fine though... and I really dont wanna go back in. i might remake the whole thing, again.
The main menu has options for:
- Addind a new contact.
- Dialing a phone number(must be saved to work).
- Viewing contacts list.
- Viewing full call history.

#### Contacts list 

Going with this option lists all saved contacts on the console. You select contacts by typing in their index numbers
Selecting a number brings up another set if options for contact methods. You can:
- Dial the selected contact.
- Edit the selected contact.
- Remove the selected contact.
- Return to the main menu.
