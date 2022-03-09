# Referrers

A referrer means a website that brings you at least one visitor. This website features a link to your shop, and thus it helps you build an audience and eventually make more sales.

![](<../../../../.gitbook/assets/43089936 (4) (4) (3).png>)

Some referrers are more important to you than others: you might have partners that have links to your shop on their own website, and both you and your partners would certainly want to know how many visitors those links brought you. You could even pay your partners to display a link to your shop, depending on how much you value your traffic.\
This, in effect, is called affiliation, and the "Referrers" page helps you build a complete affiliate program, to which even your partner can connect to see the number of visits and sales their links have generated. Registered affiliates generate traffic to your shop, you want to reward them for those visitors, and the affiliate program is how both of you can access the figures the reward is based on.

PrestaShop's referrer tool can be likened to that of a statistical dashboard open to others than only your staff members. When you create an affiliate campaign for a site, you can grant that site access to all of the activity it will have made for your site, through a password-protected URL: [http://example.com/modules/trackingfront/stats.php](http://example.com/modules/trackingfront/stats.php).

In the list of referers, the Click, Base and Percent values are calculated depending on the actual clicks, sales and percent of sales from the referer site.

## Adding a new referrer <a href="#referrers-addinganewreferrer" id="referrers-addinganewreferrer"></a>

The affiliate space enables you to create privileged access for your partners. They will have access to all statistics on the flow of visitors from their site to your online shop. To create their privileged space, you need to create their account in your affiliation program, then define how you will pay based on traffic and sales generated.

To create a new affiliate partner, click on the "Add new" button, which will take you to the affiliate creation form.

![](<../../../../.gitbook/assets/43089930 (4) (4) (3).png>)

Each section is important:

* **Affiliate**. The account of the partner in your affiliation program.
  * **Name**. To connect to your affiliation back office, your partner needs a login name; you can use a simple name or an e-mail, but make sure to use something both you and your partner can remember easily.
  * **Password**. The first time you create the account, PrestaShop saves the password along the login name. When you need to edit the account (for instance, when needing to change the commission), the password will be blank. This does not mean there is no password; if you fill the blank field when editing the account, it will change the password.
* **Commission plan**. This is where you indicate the fees of your affiliate – meaning the money you will owe your partner for actions of visitors from their site.
  * **Click fee**. This defines how much you estimate a visitor from this partner's site is worth. Every time a visitor from your partner's site comes to your shop by clicking on their link, the partner earns the marked amount.
  * **Base fee**. You can also reward your partners if visitors from their sites do buy one of your products. Note that this is only valid if the purchase is made during the browsing session that follows the click on the partner's link.
  * **Percent fee**. In addition to the base fee, or as a replacement, you can reward partners with a percentage of the sales made during the browsing session of visitors from their sites.
* **Technical information - Simple mode**. This is very important, as this is what will make the system differentiate this partner from other referrer links. Once configured, you should make a couple of test in order to make sure that you are indeed tracking the affiliate correctly.
  * **HTTP referrer**. In the "Include" field, set the partner's domain name that you want to track as your affiliate domain.
  * **Request URI**. In the "Include" field, set the last part of the query string. The system will track referrers that use a special query string. For instance, you can track referrers that use the `?prestaff=` argument in their URL. This can help you further differentiate referrers.
* **Technical information - Expert mode**. While the simple mode matches words using MySQL's "LIKE" function, the expert mode enable you to use MySQL regular expressions. This can prove very powerful but also very hard to maintain. Be sure to master the subject of regular expressions before putting anything in these fields.

![](<../../../../.gitbook/assets/43089933 (4) (4) (3).png>)

The "Help" section gives you some precious indications on how to best configure your affiliate. Read it through.

## Settings <a href="#referrers-settings" id="referrers-settings"></a>

The referrer settings are mostly tools to help you make the best of your affiliate program.

![](<../../../../.gitbook/assets/43089934 (4) (4) (2).png>)

There are three possibilities:

* **Indexing**. You must click once on the "Refresh index" button when you add a new referrer and you want to analyze your past traffic for this new referrer.
* **Cache**. PrestaShop caches the data it gathers. You can use the "Refresh cache" button to regularly refresh your data cache.
* **Save direct traffic?**. Direct traffic represents visitors who arrive on your shop directly, by typing your URL in their browser. While these are important because they are visitor who really know about your shop and are interested in your products (contrary to visitors with referrer, who might have simply stumble upon your shop by chance), saving this traffic can put a huge toll on your database. This is why this traffic is not saved nor analyzed by default. Only enable this option if you know what you are doing.
