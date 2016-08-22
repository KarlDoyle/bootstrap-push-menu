
[![NPM version](https://badge.fury.io/js/bootstrap-push-menu.svg)](http://badge.fury.io/js/bootstrap-push-menu)
[![GitHub version](https://badge.fury.io/gh/KarlDoyle%2Fbootstrap-push-menu.svg)](http://badge.fury.io/gh/KarlDoyle%2Fbootstrap-push-menu)
[![Dependency Status](https://david-dm.org/KarlDoyle/bootstrap-push-menu.svg)](https://david-dm.org/KarlDoyle/bootstrap-push-menu)
[![devDependency Status](https://david-dm.org/KarlDoyle/bootstrap-push-menu/dev-status.svg)](https://david-dm.org/KarlDoyle/bootstrap-push-menu#info=devDependencies)


![A simple mobile push menu using bootstrap 3 default menu](http://i.imgur.com/DOzXWAq.gif)
<!-- ![A simple mobile push menu using bootstrap 3 default menu](http://i.imgur.com/CXJDn7g.gif)
![A simple mobile push menu using bootstrap 3 default menu](http://i.imgur.com/RkuREuD.gif) -->
<!-- ![Angular, ES6 and Webpack Starter](http://i.imgur.com/slHDNdS.mp4) -->


bootstrap-push-menu
=============================
A custom push menu that overrides the default Bootstrap 3 mobile navigation menu.

## Quick start

Ensure you already have bootstrap 3 css loaded

```
<link rel="stylesheet" type="text/css" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
```

Link to the `bootstrap-push-menu.css` file in the head of your document

```
<link rel="stylesheet" type="text/css" href="bootstrap-push-menu.css">
```

Wrap your website in an element with the ID site-wrapper

```
<body>
  <div id="site-wrapper">
    <!-- Website goes in here -->
  </div>
</body>

```

Add the default bootstrap navigation

```
<body>
  <div id="site-wrapper">

    <!-- Navigation follows bootstrap navbar component -->
    <nav class="navbar navbar-default">
      <div class="container-fluid">
        <div class="navbar-header">
          <button type="button" class="collapsed navbar-toggle" data-toggle="collapse" aria-expanded="false">
            <span class="sr-only">Toggle navigation</span>
            <span class="icon-bar"></span>
            <span class="icon-bar"></span>
            <span class="icon-bar"></span>
          </button>
          <a href="#" class="navbar-brand">Brand</a>
        </div>
        <div class="collapse navbar-collapse">
          <ul class="nav navbar-nav">
            <li class="active"><a href="#">Link <span class="sr-only">(current)</span></a></li>
            <li><a href="#">Link</a></li>
            <li><a href="#">Link</a></li>
            <li><a href="#">Link</a></li>
          </ul>
        </div>
      </div>
    </nav>
    <!-- Website goes in here -->
  </div>
</body>

```

Add a javascript targeting `.navbar-toggle` to toggle `<body class="open">`
Here i am using jQuery, but you can choose any method you prefer.

```
  <!-- Added jQuery to demonstrate example -->

  <script src="https://code.jquery.com/jquery-2.2.4.min.js" integrity="sha256-BbhdlvQf/xTY9gja0Dq3HiwQF8LaCRTXxZKRutelT44=" crossorigin="anonymous"></script>

  <script>
    $(document).ready(function() {
      $(document).on('click', '.navbar-toggle', function(event) {
        event.preventDefault();
        $('body').toggleClass('open');
      });
    });
  </script>
```

here is a [link](_demo/) to the demo


## Support / Contact / Suggestions

I am interested in hearing your feedback and to answer any questions you may have.

Contact me [here](https://github.com/KarlDoyle/bootstrap-push-menu/issues)

Thank You



