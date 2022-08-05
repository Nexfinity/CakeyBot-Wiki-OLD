# Verification Role

{% hint style="warning" %}
Make sure that Cakey Bot has **`Manage Roles`** permission.

Also, ensure that Cakey Bot's role is _above_ the verification role you want Cakey bot to give users.
{% endhint %}

## Verification Command

You can force users to run the `/verify` command in order to be granted a role that you have selected. This is a great way to make sure users read any rules or important info you have before they are able to chat in your server. Users will only need to type the`/verify` command in order to get the role.&#x20;

In order to set the role that you want users to get, you will need to type `/setup verifyrole <role>`. You can also disable or remove the role by typing `/setup verifyrole 0`. If you want to change the role later, you can just run the initial setup command and type the new role and it will update the currently saved role.

{% hint style="success" %}
**Helpful Tip:** You can also set the verification role in the [web dashboard](https://cakeybot.app/dashboard/public)!
{% endhint %}
