# Verification Role

{% hint style="warning" %}
Make sure that Cakey Bot has the **`Manage Roles`** permission if you are using the setup portion of the command.

Also, ensure that Cakey Bot's role is _above_ the verification role you want Cakey bot to give users.
{% endhint %}

## Verification Command

You can force users to run the `!verify` command in order to be granted a role that you have selected. This is a great way to make sure users read any rules or important info you have before they are able to chat in your server. Users will only need to type the`!verify`command in order to get the role. In order to set the role that you want users to get, you will need to type `!verify setup <role>`. You can also disable or remove the role by typing `!verify setup none`. If you want to change the role later on, you can just run the initial setup command and type the name or id of the new role and it will update the currently saved role.

{% hint style="success" %}
**Helpful Tip:** You can also set the verification role in the [web dashboard](https://cakeybot.app/dashboard/public)!
{% endhint %}

