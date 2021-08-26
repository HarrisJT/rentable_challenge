======================================
  Gilded Rose Requirements Specification
======================================

Hi and welcome to team Gilded Rose. As you know, we are a small inn with a prime location in a
prominent city ran by a friendly innkeeper named Allison. We also buy and sell only the finest goods.

Your task is to add the new feature to our system so that
we can begin selling a new category of items. First an introduction to our system:

	- All items have a sell_in value which denotes the number of days we have to sell the item
	- All items have a quality value which denotes how valuable the item is
	- At the end of each day our system lowers both values for every item

Pretty simple, right? Well this is where it gets interesting:

	- Once the sell by date has passed, quality degrades twice as fast
	- The quality of an item is never negative
	- "Aged Brie" actually increases in quality the older it gets
	- The quality of an item is never more than 50
	- "Sulfuras", being a legendary item, never has to be sold or decreases in quality
	- "Backstage passes", like aged brie, increases in quality as its sell_in value approaches;
	quality increases by 2 when there are 10 days or less and by 3 when there are 5 days or less but
	quality drops to 0 after the concert

Just for clarification, an item can never have its quality increase above 50, however "Sulfuras" is a
legendary item and as such its quality is 80 and it never alters.

## We have recently signed a supplier for a new "conjured" item. Please implement the following:

  - "*Conjured Mana Cake*": **quality** degrades by 2 per day before the **sell_in**
  date has passed and by 4 after. Its **sell_in** decreases by one every day. Its quality can never decrease to less than 0.

Feel free to make any changes to the UpdateQuality method and add any new code as long as everything
still works correctly.

## The tests work and are fully comprehensive. Use them!
