<script>
    import { Page, GridLayout, Label } from '@nativescript/core';
</script>

<page>
    <actionBar title="Home" class="action-bar">
        <image src="~/assets/archa.png" width="40" height="40"></image>
    </actionBar>

	<tabView>
		<tabViewItem title="Home">
				<label textWrap="true">Coming soon... hopefully</label>
		</tabViewItem>
		<tabViewItem title="Battlepass">
				<label textWrap="true">Coming soon as well...</label>
		</tabViewItem>
		<tabViewItem title="Battlepass">
			<label textWrap="true">Coming soon as well...</label>
		</tabViewItem>
		<tabViewItem title="Search">
			<label textWrap="true">Coming soon as well... maybe</label>
		</tabViewItem>
		<tabViewItem title="User Profile">
			<label textWrap="true">Coming soon as well...</label>
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

	actionBar {
		background-color: #b8ff00;
	}
</style>
