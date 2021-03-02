# bestbuy-queue-automation
Simple Tampermonkey script for automating Best Buy's product queue.  
New version lints fine but is untested (adds auto-reload on unavailable / sold out products), if you're interested [download the source here](https://github.com/albert-sun/bestbuy-queue-automation/tree/a9708d65dc65e939fd4615f247efc390f3622cd0) and test it out for yourself. Thank you!

# Frequently Asked Questions
**Q: Does this script work on non-focused tabs?**
A: The script runs as long as the tab has been focused once (for instance, if you click "Open in new tab" you would have to navigate to the tab). The script also only works during the queue, so make sure to press the initial "Add to Cart" button to initiate the queue (you should see the bottom left status change).  

**Q: How do I know the script is running?**
A: You can either check the TamperMonkey or GreaseMonkey icon (it should have a little red [1] signifying the script is active), or you can check for the red-orange banner at the bottom of the product page. Keep in mind that the script currently only functions on individual product pages and not on search results or the saved items page.

# Instructions
Install the script through the TamperMonkey extension for Chrome or the GreaseMonkey extension for Firefox.  
[Copy the contents of the script here as a new script into the above extensions](https://github.com/albert-sun/bestbuy-queue-automation/blob/main/script.js).  
- The script automatically runs on page load (a red-orange banner should appear)
- You only have to press the initial "Add to Cart" button if you don't have initialClick enabled in the script config.
- At that point, when the queue pops the button will automatically click, play a sound, and open the cart window!
