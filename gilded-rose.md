Gilded Rose
===========
Hi and welcome to team **Gilded Rose**. 
As you know, we are a small inn with a prime location in a prominent city run by a friendly innkeeper named **Allison**.
We also buy and sell only the finest goods.
Unfortunately, our goods are constantly degrading in quality as they approach their sell by date. 
We have a system in place that updates our inventory for us. 

It was developed by a guy named Leeroy, who has moved on to new adventures. 
Your task is to add the new feature to our system so that we can begin selling a new category of items. 

## Introduction to our system:

* All items have a `sell_in` value which denotes the number of days we have to sell the item.
* All items have a `quality` value which denotes how valuable the item is.
* At the end of each day our system lowers both values for every item using the method `update_quality`.

Pretty simple, right? Well this is where it gets interesting:

* Once the sell by date has passed, `quality` degrades twice as fast.
* The `quality` of an item is never negative.
* "Aged Brie" increases in `quality` the older it gets.
* The `quality` of an item is never more than 50.
* `Sulfuras` is a legendary item and as such its `quality` is always 80 and it never alters.
* "Backstage passes", like "Aged Brie", increases by one in `quality` as its SellIn date approaches
    - `quality` increases by 2 when there are 10 days or less 
    - `quality` increases by 3 when there are 5 days or less 
    - `quality` drops to 0 after the concert

## The requirement

We have recently signed a supplier of conjured items. This requires AN UPDATE to our system:

 - "Conjured" items degrade in `quality` twice as fast as normal items

Feel free to make any changes to the `update_quality` method and add any new code as long as everything still works correctly. 
However, **do not alter the Item class or Items property** as those belong to the goblin in the corner who will insta-rage and one-shot you as he doesn't believe in shared code ownership.

## Final Notes

Just for clarification: an item can never have its `quality` increase above 50.
