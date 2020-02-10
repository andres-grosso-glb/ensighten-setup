# 1. Create a new space

1. Log in to Ensighten Manage.
2. Click **Spaces** from left menu.
3. Click **Add Space** and enter your space info.
4. Publish your changes and make a note of the Bootstrap include script.

{% hint style="success" %}
**Best Practices for creating a new space**

* Create a space per environment: **production** and **non-production** environments.
* Add a server side **kill switch** for the Bootstrap. In case of the Ensighten causing any issues on the site, you can easily take it out.
* Add an **environment logic** to automatically load production vs non-production Bootstrap.
* Enable **Tag Alerts** and **Publish Alerts** \(Click **turnerintl** in the top right and select **settings**\), so you get a notification email when someone publishes in your space.
{% endhint %}

#### Example Bootstrap

```text
<script type="text/javascript" src="//nexus.ensighten.com/turnerintl/example-space/Bootstrap.js"></script>
```



