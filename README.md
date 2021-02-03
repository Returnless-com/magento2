<p align="center">
  <img src="https://www.returnless.com/media/retour-integratie-magento-2.png" width="450"/>
</p>
<h1 align="center">Returnless Connector for Magento 2.2.x and higher</h1>


<h2>Install using Composer</h2>
Step-by-step to install the Returnless Connector for Magento® 2 by Composer:

1. Open your your SSH Console to connect to your Magento® 2 store. Once connected, locate the root of your Magento® 2 store.

2. Enter the command line in your Root and wait as composer will download the extension for you:

<pre>composer require returnless-com/magento2</pre>

3. When it’s finished you can activate the extension and clean the caches using the following command line;

<pre>
php bin/magento module:enable Returnless_Connector
php bin/magento setup:upgrade
php bin/magento cache:clean
</pre>

4. If Magento® is running in production mode, please also deploy the static content:

<pre>
php bin/magento setup:static-content:deploy
</pre>

5. Create a new integration Authentication token to give us access to your store. 
In your Magento® 2 backend, go to <strong>System > Integrations</strong> and click <strong>Add New Integration</strong>.
Enter the following details:
- Name: Returnless Connector
- Your password: your admin password
- (API tab) Resource Access: All

6. Save the integration. Click <strong>Activate</strong> and click <strong>Allow</strong>.

7. Save the <i>Access Token</i> and send it to your Returnless contact person so we can connect the return form to your store.

 
## About Returnless ##
With Returnless, you can easily automate and optimize your return proces by setting up a custom return form for your e-commerce webshop. We can help you to reduce your returns costs and -percentage, while making your consumers happy with a unique return experience.

Using the Returnless Connector for Magento 2, you can connect your return form with your Magento 2 backend, so that we can load the order information from your store. A customer will enter the order increment ID + customer emailaddress so that we can load all relevent order items related to the order. To use the Magento Connector, you will need a [Pro subscription](https://www.returnless.com/tarieven) for Returnless.
  

## Supported features of the Returnless Connector ##
- Load order info from your return form by Magento Increment ID.
- Validate order by customer email address.
- Load order items related to order.
- Load product information (e.g. product images) related to order items.

<p align="center">
  <img src="https://www.returnless.com/media/iphone-retourformulier-shirtstore.jpg" width="450"/>
</p>


## Configuration, FAQ and Troubleshooting  ##
If you experience problems with the extension installation, setup or whenever you need more information about how to setup the Returnless Connector extension in Magento 2.2.x and higher, please send an e-mail to [developer@returnless.com](mailto:info@returnless.com) and we will help you through the process.


## License ##
[BSD (Berkeley Software Distribution) License](http://www.opensource.org/licenses/bsd-license.php).
Copyright (c) 2018-2020, Returnless
