Magento-Order-Status-Image
==========================
Better Order Status on Order Page
This module uses a better/cuttier way to display order status on customer order page view.

## Screenshot

![ScreenShot](https://raw.githubusercontent.com/blopa/Magento-Order-Status-Image/master/screenshot/screenshot.jpg)

## Instalation

1. Open the file ```path/to/magento/app/design/frontend/default/default/template/sales/order/info.phtml``` and around line 52, right after div ```order-info``` add the code ```<?php echo $this->getLayout()->createBlock('core/template')->setTemplate('werules/orderstatus/status.phtml')->toHtml(); ?>```.

2. Upload the content from Magento-Root folder to your magento root directory 

Now you are ready to go!

## Obs

It's possible that you have a custom template and it will not use the standard info.phtml from magendo base, so you need to check which file you're using to edit, you can easily do that by switching on the template hints on magento admin panel