# Beginning Scala session2

------

1. Modify the Checkout System from your previous session.

    a. "Banana costs N450.50 and Avocado costs N725.60.
    Scanning an Apple, Banana and Avocado should be 1476.10"

    b. We want to be able to set up special offers in the checkout system. E.g Buy X fruits and it will cost you Y Naira.
    Here is the current offer list:


         Item   Unit      Special
                Price     Price
         --------------------------
         Apple     300       3 for 800
         Orange    150       2 for 200
         Banana    450.50
         Avocado   725.60

    Our checkout accepts items in any order, so that if we scan an Orange, a Banana, and another Orange, we’ll recognize the two Oranges and price them at 200
    (for a total price so far of 650.50). Because the pricing changes frequently,
    we need to be able to pass in a set of pricing rules each time we start handling a checkout transaction.
    Your interface should look something like this :

    CheckoutSystem.getTotal(offers)(items)

    Using the above offers, write unit tests for

        i. 1 Apple, 1 Orange, 2 Bananas and 1 Avocado
        ii. 4 apples and 3 Oranges
        iii. 2 Oranges and 2 Avocados

    c. Market prices have changed. We have new special offers list, as below

             Item   Unit      Special
                        Price     Price
                 --------------------------
                 Apple     300
                 Orange    150
                 Banana    450.50    2 for 800
                 Avocado   725.60    2 for 1400


     Using this updated offer list, write unit tests for

            i. 1 Apple, 1 Orange, 2 Bananas and 1 Avocado
            ii. 4 apples and 3 Oranges
            iii. 2 Oranges and 2 Avocados

