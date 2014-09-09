# ip-geo-locator
[Polymer][polymer] web component for locating geographic location of an IP address.

## Install

```bash
bower install --save mbykovskyy/ip-geo-locator
```

## Usage

```html
<link rel="import" href="ip-geo-locator.html">

<ip-geo-locator id="locator"></ip-geo-locator>
Your approximate location is: <pre id="output"></pre>

<script>
  var locator = document.getElementById('locator');

  locator.addEventListener('location-changed', function() {
    var output = document.getElementById('output');
    output.innerHTML = JSON.stringify(locator.location, null, 2);
  });
</script>
```

See [component page][ip-geo-locator] for details and demo.

[polymer]: http://polymer-project.org "Polymer"
[ip-geo-locator]: http://mbykovskyy.github.io/ip-geo-locator "Component Page"
