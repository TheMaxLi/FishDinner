<script>
	import Chefs from '../components/Chefs.svelte';
	import Faq from '../components/Faq.svelte';
	import Footer from '../components/Footer.svelte';
	import Header from '../components/Header.svelte';
	import HeroImage from '../components/HeroImage.svelte';
	import InfoSection from '../components/InfoSection.svelte';
	import MapSection from '../components/MapSection.svelte';
	import Menu from '../components/Menu.svelte';
	import Navigation from '../components/Navigation.svelte';
</script>

<div class="w-96 min-h-screen bg-gradient-to-b from-white to-sky-400 font-['New_Spirit']">
	<Header />
	<Navigation />
	<HeroImage />
	<Chefs />
	<Menu />
	<InfoSection />
	<MapSection />
	<Faq />
	<Footer />
</div>
