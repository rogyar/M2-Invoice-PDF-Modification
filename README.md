# Edit Magento 2 invoice PDF example

---

## Description
The module demonstrates the invoice PDF modification in a scope of Magento 2 project. The following items are changed:

* Changed the invoice header background from grey to white
* Added product image to the products list

The module is created as an example for SO [question](https://magento.stackexchange.com/questions/179587/how-to-get-product-image-remove-background-color-on-pdf-invoice-magento-2-x).
 There are plenty of ways to optimize the solution. The code represented here it's just quick workaround that can be 
  used as a basis for further development.
  
## Installation

* Copy the files into the newly created directory `app/code/Atwix/InvoiceMod`
* Clean the cache, enable module and run setup:upgrade command

## Known issues
Unfortunately, the PDF generation logic in M2 is not as flexible as the other parts of the system. So, a tons of code need
to be overridden. The code does not contain the line height modification of the order items list.

## Compatibility
Tested on Magento 2.1.*