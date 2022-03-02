<script>
  import {link} from 'svelte-routing'
</script>

<nav class="navbar navbar-expand-lg navbar-dark bg-primary shadow">
  <div class="container-xxl">
    <a class="navbar-brand" href="/" use:link>Navbar</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="/" use:link>Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="/about" use:link>About</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="/products" use:link>Products</a>
        </li>
        <!-- <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" id="navbarDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            Products
          </a>
          <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
            <li><a class="dropdown-item" href="/products/1">Action</a></li>
            <li><a class="dropdown-item" href="/products/2">Another action</a></li>
            <li><hr class="dropdown-divider"></li>
            <li><a class="dropdown-item" href="/products/3">Something else here</a></li>
          </ul>
        </li> -->
      </ul>
    </div>
  </div>
</nav>