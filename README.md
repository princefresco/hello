START

DECLARE productName[12] AS STRING
DECLARE productPrice[12] AS FLOAT
DECLARE productNumber AS INTEGER
DECLARE quantity AS INTEGER
DECLARE totalPrice AS FLOAT

DISPLAY "FM GROCERY"
DISPLAY "[1] Corned Beef (150g) - P70.12"
DISPLAY "[2] 555 Tuna (155g) - P45.23"
DISPLAY "[3] Century Tuna (155) - P75.11"
DISPLAY "[4] Gardenia Classic WB (600g) - P90.42"
DISPLAY "[5] Gardenia High Fiber WB (400g) - P93.76"
DISPLAY "[6] SariMonde Tasty Bread (450g) - P91.12"
DISPLAY "[7] Nagaraya (160g) - P49.42"
DISPLAY "[8] Potato Fries Ketchup (35g) - P65.59"
DISPLAY "[9] Oishi Pillows Choco (38g) - P14.21"
DISPLAY "[10] Alfonso Light (1L) - P290.42"
DISPLAY "[11] Alfonso Platinum (1L) - P380.53"
DISPLAY "[12] RedHorse (100ml) - P90.21"

INPUT "Product Number: " TO productNumber

IF productNumber >= 1 AND productNumber <= 12 THEN
    DISPLAY "You selected: " + productName[productNumber]
    DISPLAY "Price: P" + productPrice[productNumber]

    INPUT "Enter Quantity: " TO quantity

    IF quantity > 0 THEN
        SET totalPrice = productPrice[productNumber] * quantity
        DISPLAY "Quantity: " + quantity
        DISPLAY "Total Price: P" + totalPrice
    ELSE
        DISPLAY "Error: Invalid Quantity!"
END



























      

ELSE
    DISPLAY "Error: Invalid Product Number!"

END
