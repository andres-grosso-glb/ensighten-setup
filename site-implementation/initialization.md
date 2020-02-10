# Initialization

A global standards implementation starts with two steps. In the `<head>` of every page:

1. Add a JavaScript Object named **turner\_metadata** with an empty **trackAction** array.
2. Add a call to an external JavaScript file; the Ensighten **Bootstrap.js**.

{% hint style="success" %}
**Turner Metadata Object**  
  
In the context of HTML based content \(e.g., web sites\), the **turner\_metadata** object is:

* A window-scoped variable
* Defined as turner\_metadata
* Follows JSON Syntax
* Must contain trackAction array
{% endhint %}

{% hint style="info" %}
**OneTrust Banner**  
  
OneTrust banner script should be implemented by the site dev team. Analytics team does not provide the script.  
Once the OneTrust banner has implemented, **OnetrustActiveGroups** variable should be created, and it must contain at least one of the following category IDs:

* Category 1 - Strictly Necessary
* Category 2 - Performance
* Category 3 - Functional
* Category 4 - Targeting
* Category 8 - Social Media

**Best Practices:**

* Implement the black veil overlay, so the users cannot navigate into the site until they agree to the user consent.
* Reload the page once the users agree to the user consent, so you can capture the initial pageview.
{% endhint %}

#### Example Code:

```text
<html>
  <head>
      <script>
          var turner_metadata = {
              "trackAction" : []
          };
      </script>
      <script src="//nexus.ensighten.com/turnerintl/example-space/Bootstrap.js"></script>
  </head>
</html>
```

