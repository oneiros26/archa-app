<script>
	import Ticket from './Ticket.svelte';
	import Search from './Search.svelte';
	import Messagenig from './Messagenig.svelte';
	import Profile from './Profile.svelte';
	import RealHome from './RealHome.svelte';
</script>

<page class="red">
    <actionBar title="Home" class="action-bar">
        <image src="~/assets/archa.png" width="40" height="40"></image>
    </actionBar>

	<tabView androidTabsPosition="bottom" androidSelectedTabHighlightColor="#b8ff00" tabTextColor="#b8ff00" tabBackgroundColor="#0f0f0f" selectedTabTextColor="#f0f0f0">
		<tabViewItem title="" class="fas tab_size">
			<RealHome />
		</tabViewItem>
		<tabViewItem title="" class="fas tab_size" >
			<Ticket />
		</tabViewItem>
		<tabViewItem title="" class="fas tab_size">
			<Search />
		</tabViewItem>
		<tabViewItem title="" class="fas tab_size">
			<Messagenig />
		</tabViewItem>
		<tabViewItem title="" class="fas tab_size">
			<Profile />
		</tabViewItem>
	
	</tabView>
</page>

<style>
	:root {
		--c_primary: #b8ff00;
		--c_primary_dark: #ff4c00;
		--c_dark: #0f0f0f;
		--c_light: #f0f0f0;

		--c_text: #000;
		--c_text_light: #fff;

		--c_purple: #ac71ff;
		--c_pink: #ff78d9;
		--c_orange: #ff4c00;
		--c_green: #64d13e;
		--light_blue: #76a8ff;
	}
	.tab_size {
		font-size: 25;
	}
	actionBar {
		background-color: #b8ff00;
	}
</style>
