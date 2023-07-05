# Security

## Back office token protection

The token protection helps **secure access to your back office by using tokens**.&#x20;

<details>

<summary>Learn more about Back Office Token Protection </summary>

When this feature is enabled, each URL becomes specific to a customer's session, and cannot be used as-is on another browser, thus protecting any information they might have stored during that session.

By default, back office token protection is **enabled.**

</details>

### Configure the password policy & password strength indicator

The **password policy** menu allows you to configure your store's password policy by choosing between 5 increasing levels of complexity. This will allow you to decide how strict you want to be about user passwords.&#x20;

Passwords are rated from **0** (Extremely guessable) to **4** (Very unguessable) based on their security score. The minimum and maximum length of passwords can be set manually.

<figure><img src="../../../.gitbook/assets/image (84).png" alt=""><figcaption></figcaption></figure>

When creating an account, front office users receive real-time cues of their chosen password’s strength according to the back office password policy. A color-coded cue _–_ as well as a tooltip _–_ will help them understand if their password is strong enough.

_**Note:** themes must be updated to support this feature. See_ [#themeandlogo-yourcurrenttheme](../../improving-shop/customizing-store-design/theme-and-logo.md#themeandlogo-yourcurrenttheme "mention")

| Cue color | Password length | Password strength |
| :-------: | :-------------: | :---------------: |
|     🟥    | Not long enough | Not strong enough |
|     🟧    | Not long enough |       Strong      |
|     🟩    |       Good      |       Strong      |

|        An example of a weak password (🟥,🟧)       |        An example of a strong password (🟩)        |
| :------------------------------------------------: | :------------------------------------------------: |
| ![](<../../../.gitbook/assets/image (87) (1).png>) | ![](<../../../.gitbook/assets/image (58) (1).png>) |

## Manage employee and customer sessions

These tabs allow you to **manage employee and customer sessions**. To delete a session and sign out the user, click on the delete button in the Actions column.

To access the back office, the employee or customer will need to sign back in using their email and password.

<figure><img src="../../../.gitbook/assets/image (76) (1).png" alt=""><figcaption><p>The <strong>Employee Sessions</strong> tab allows you to manage employee sessions.</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (81) (1).png" alt=""><figcaption><p>The <strong>Customer Sessions</strong> tab allows you to manage customer sessions.</p></figcaption></figure>

### Clear outdated Sessions

The Clear button allows you to manually delete outdated sessions to reduce database clutter.

<figure><img src="../../../.gitbook/assets/image (72) (1).png" alt=""><figcaption></figcaption></figure>
