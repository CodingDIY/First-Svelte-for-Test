<script>
	// Routing
	import {Router, Link, Route} from 'svelte-routing'

	// Pages
	import Login from './pages/Login.svelte'
	import Checkout from './pages/Checkout.svelte'
	import Products from './pages/Products.svelte'
	import ProductTemplate from './pages/ProductTemplate.svelte'
	import Home from './pages/Home.svelte'
	import About from './pages/About.svelte'

	// Components
	import Navbar from './components/Navbar.svelte'
</script>

<!-- Router link issue: https://stackoverflow.com/questions/68655730/page-not-found-issue-when-directly-visit-the-link-in-svelte-routing -->
<Router>
	<Navbar />
	<Route path='/' component={Home} />
	<Route path='/about' component={About} />
	<Route path='/login' component={Login} />
	<Route path='/checkout' component={Checkout} />
	<Route path='/products' component={Products} />
	<Route path='/products/:id' component={ProductTemplate} />
</Router>
