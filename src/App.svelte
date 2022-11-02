<script>
	export let name;


	import Home from '../Component/Home/Home.svelte';
	import Contact from '../Component/Contact/Contact.svelte';
	import Header from '../Component/Header/Header.svelte';
	import Login from '../Component/Login/Login.svelte';
	import SignIn from '../Component/SignIn/SignIn.svelte';
	import Mainpage from '../Component/Mainpage/Mainpage.svelte';
	import Group from '../Component/Group/Group.svelte';
	import Log from '../Component/Log/Log.svelte';
	

	import Router from 'svelte-spa-router';

	const routes={
		'/':Home,
		'/Contact1':Contact,
		'/Contact2/test':Contact,
		'/Login':Login,
		'/SignIn':SignIn,
		'/Mainpage':Mainpage,
		'/Group':Group,
		'/Log':Log,
	};
</script>

<main>
	<Header />
	<Router {routes}/>

	<h1>Hello {name}!</h1>

</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>