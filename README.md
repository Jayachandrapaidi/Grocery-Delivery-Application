**Featured on [CNBC](https://www.cnbc.com/2020/04/08/how-to-get-a-amazon-fresh-whole-foods-delivery-timeslot.html)**

#### Quick Links
- [Download & Instructions](#instructions)
- [Disclaimer about 'disappearing' slots](#disclaimer-about-disappearing-slots)
- [Questions/feedback/issues](https://github.com/ahertel/Amazon-Fresh-Whole-Foods-delivery-slot-finder/issues)
- [Track bugs/enhancements](https://github.com/ahertel/Amazon-Fresh-Whole-Foods-delivery-slot-finder/projects)
- [Supporting me/Donations](#supporting-medonations)

# Amazon Fresh/Whole Foods Delivery Slot Finder
A Mac-only tool that finds available delivery slots for Amazon.com's Whole Foods delivery and Amazon Fresh services.

## New Features
* #### New interface - added 4/6/20
  * Improve user experiecnce to accompany new features
* #### Text message notifications - added 4/6/20
  * You can now get text messages when a slot is found. Added by popular demand, despite limitated utility: If you set the recipient to the same number linked to your Mac's 'Messages' app, you may not be notified on your phone as the texts may be automatically marked as read. Thus it's recommended that you enter a different phone number from the one linked to your 'Messages' app (e.g your google voice number that forwards to your real number, a family member's number, your work cell-phone)
* #### Automatically handle unknown pages - added 4/6/20
  * Amazon.com sometimes redirects the URL of the delivery slot page to the Amazon homepage, and previously the tool would require a manual restart. Now it automatically navigates back the delivery slot page whenever an unknown page is encountered. One step closer to this program running without needing any monitoring/intervention

* #### Auto-ignore out of stock items -  added 3/31/20
  * Amazon.com displays notices when items in your cart go out of stock. Now the tool can automatically ignore these warnings so it keep looking for slots without your intervention.


## DISCLAIMER about "disappearing" slots
No guarantee that slots will be found and/or that slots will work. Often you will select a slot but the page will refresh and the slot will disappear. These phantom slots are very common and are unfortunately in Amazon's control, not mine.  Eventually a slot should work. Some users report success of after 20+ tries. Wishing you resilience and hope! Feel free to post concerns in the [Issues](https://github.com/ahertel/Amazon-Fresh-Whole-Foods-delivery-slot-finder/issues) section.

## Instructions
1. Read the [Compatibility](#compatibility) section below to make sure the tool will work for you
2. Download the 'delivery-window-finder.scpt' [here](https://github.com/ahertel/wholefoods-delivery-slot-finder/raw/master/delivery-window-finder.scpt)
3. Enable "Allow JavaScript from Apple Events". [How-to video](https://www.youtube.com/watch?v=S6zb_6yTAbo)
4. Log into your Amazon account in Safari
5. Fill your Whole Foods/Amazon Fresh cart with your complete order and proceed through the checkout process manually. Stop once you've arrived at the page saying no slots are available
6. Open delivery-window-finder.scpt in _Script Editor_ and click the 'Play' button to run it and follow the prompts
![run button](https://i.imgur.com/kpQee5h.png)
7. Turn up the volume to hear the notification when a slot is found
8. Once you receive your order, please consider tipping if you can. They are exposing themselves to risk to protect us. Thanks!

Notes:
The script will stop running if your computer falls asleep. You can adjust your 'Energy Saver' settings in System Preferences or download [Caffeine app](https://intelliscapesolutions.com/apps/caffeine) to keep your Mac awake.

## Compatibility
Currently **not compatible** with Whole Foods orders from primenow.amazon.com. Currently only compatible with Amazon Fresh and Whole Foods orders from amazon.com. Prime Now compatibility may be added eventually. Check [here](https://github.com/ahertel/Amazon-Fresh-Whole-Foods-delivery-slot-finder/issues/23) for any progress.

**Before using this tool**, ensure that your checkout page looks **exactly** like the examples in the _Compatible_ section below.
This tool currently only works for some regions because Amazon's checkout pages seem to vary based on your location and I designed the tool based on the page I see in my region. 
If your checkout page doesn't look like the examples in the _Compatible_ or _Incompatible_ sections below, this tool may still work for you but no guarantees.

### Compatible
These are sample screenshots for delivery to a New Jersey address
#### Whole Foods
![Whole Foods](https://i.imgur.com/r7EQQF6.jpg)

#### Amazon Fresh
![Amazon Fresh](https://i.imgur.com/ncVyqQR.jpg)

### Incompatible
#### Amazon Fresh
##### 1.
![Santa Clara, CA](https://i.imgur.com/SyNtrZs.png)
##### 2.
![an unkown city in CA](https://i.imgur.com/PYrO9Il.jpg)


## How it works
- It opens the checkout page in a new window, minimizes it, and then refreshes every ~60 seconds in the background.
- Once it finds an open slot it alerts you by putting a notification on your screen and playing a sound, and opening the checkout page. You can choose to receive text messages when a slot is found
- You can choose to have the tool ignore out of stock notifications and continue searching uninterrupted
- Once you're notified, quickly select a slot and finish checking out because available slots are snagged almost instantly.

## Inspiration for this tool
The Coronavirus 2019 pandemic caused a surge in demand for grocery delivery services, making it nearly impossible to find an open delivery slot. My intention in providing this tool is first and foremost help those in need (e.g. at-risk people, health care workers) have an easier time staying safe. The idea came to me when I realized my parents, who both have auto-immune diseases, had been trying unsuccesfully for several days to get grocery delivery slots.
