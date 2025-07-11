<script>
	import Chefs from '../components/Chefs.svelte';
	import Faq from '../components/Faq.svelte';
	import Footer from '../components/Footer.svelte';
	import Header from '../components/Header.svelte';
	import TheGoat from '../components/TheGoat.svelte';
	import InfoSection from '../components/InfoSection.svelte';
	import MapSection from '../components/MapSection.svelte';
	import Menu from '../components/menu/Menu.svelte';
	import Navigation from '../components/Navigation.svelte';
</script>

<div class="w-screen min-h-screen font-['New_Spirit']">
	<Header />
	<Navigation />
	<TheGoat />
	<Chefs />
	<Menu />
	<InfoSection />
	<!-- 
	<MapSection />
	<Faq />
	<Footer /> 
	-->
</div>
