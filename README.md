START

DECLARE productName[12] AS STRING
DECLARE productPrice[12] AS FLOAT
DECLARE productNumber AS INTEGER
DECLARE quantity AS INTEGER
DECLARE totalPrice AS FLOAT
DECLARE date AS STRING
DISPLAY "=================================================="
DISPLAY " FM GROCERY"
DISPLAY "=================================================="
DISPLAY "[PRODUCTS] DATE: " + date
DISPLAY "----------------------CANNED------------------------"
DISPLAY "[1] " + productName[1] + " - P" + productPrice[1]
DISPLAY "[2] " + productName[2] + " - P" + productPrice[2]
DISPLAY "[3] " + productName[3] + " - P" + productPrice[3]
DISPLAY "---------------------PASTRIES-----------------------"
DISPLAY "[4] " + productName[4] + " - P" + productPrice[4]
DISPLAY "[5] " + productName[5] + " - P" + productPrice[5]
DISPLAY "[6] " + productName[6] + " - P" + productPrice[6]
DISPLAY "----------------------SNACKS------------------------"
DISPLAY "[7] " + productName[7] + " - P" + productPrice[7]
DISPLAY "[8] " + productName[8] + " - P" + productPrice[8]
DISPLAY "[9] " + productName[9] + " - P" + productPrice[9]
DISPLAY "---------------------ALCOHOL------------------------"
DISPLAY "[10] " + productName[10] + " - P" + productPrice[10]
DISPLAY "[11] " + productName[11] + " - P" + productPrice[11]
DISPLAY "[12] " + productName[12] + " - P" + productPrice[12]
DISPLAY "=================================================="

INPUT "Product Number: " TO productNumber

IF productNumber >= 1 AND productNumber <= 12 THEN
    DISPLAY "You selected: " + productName[productNumber]
    DISPLAY "Price: P" + productPrice[productNumber]

    INPUT "Enter Quantity: " TO quantity

    IF quantity > 0 THEN
        SET totalPrice = productPrice[productNumber] * quantity
        DISPLAY "Total Price: P" + totalPrice
    ELSE
        DISPLAY "Error: Invalid Quantity! Quantity must be greater than 0."

ELSE
    DISPLAY "Error: Invalid Product Number! Please choose from 1-12 only."
END








END
