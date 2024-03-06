# Create a Navigation 
This is a simple example of a responsive Bootstrap 4 navbar with an icon. It includes the necessary HTML, CSS, and JavaScript to create a functioning navbar that collapses into a toggleable menu on smaller screens

```
<nav class="navbar navbar-expand-md navbar-dark">
  <div class="container">
    <!-- Brand/logo -->
    <a class="navbar-brand" href="#">
      <i class="fas fa-code"></i> Your Logo
    </a>

    <!-- Toggler/collapsibe Button -->
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#collapsibleNavbar">
      <span class="navbar-toggler-icon"></span>
    </button>

    <!-- Navbar links -->
    <div class="collapse navbar-collapse" id="collapsibleNavbar">
      <ul class="navbar-nav ml-auto">
        <li class="nav-item">
          <a class="nav-link" href="#">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">About</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Services</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Contact</a>
        </li>
      </ul>
    </div>
  </div>
</nav>

```

Replace your-icon-url with the URL of your desired icon.

Add the following CSS to your stylesheet:

```
* {
    font-family: 'Poppins', sans-serif;
  }

  .navbar {
    background-color: #30475e; 
  }

  .navbar-brand {
    color: #ffffff;
    font-weight: bold;
  }

  .navbar-nav .nav-item .nav-link {
    color: #fff;
    position: relative; 
    transition: 0.3s;
    font-weight: 400;
    color:#fff;
  }

  .navbar-nav .nav-item .nav-link::before {
    content: '';
    position: absolute;
    width: 0%;
    height: 2px;
    bottom: 0;
    left: 0;
    background-color: #f8b739;
    transition: 0.3s;
    color:#fff;
  }

  .navbar-nav .nav-item .nav-link:hover::before {
    width: 100%; 
    color: #fff;
  }

```

