<script>
	import { writable } from 'svelte/store';
	let textElem = '';
	let messages = writable([]);

	function sendMessage() {
		if (textElem) {
			messages.update((msgs) => [...msgs, textElem]);
			console.log(textElem);
			textElem = '';
		}
	}
</script>

<absoluteLayout>
	<label textWrap="true" marginLeft="100" top="0" text="Ahoj, včera jsem viděl Hamleta" backgroundColor="#64d13e" />
	<label textWrap="true" marginLeft="62" top="50" text="Musím říct, že to bylo fenomenální!" backgroundColor="#64d13e" />
	<label textWrap="true" marginLeft="20" top="110" text="Já na tom byl minulý měsíc" backgroundColor="#76a8ff" />
	<label textWrap="true" marginLeft="20" top="160" text="úplně mě dostala scéna s duchem!" backgroundColor="#76a8ff" />
	<label textWrap="true" marginLeft="255" top="220" text="To zní super!" backgroundColor="#ff4c00" />
	<label textWrap="true" marginLeft="92" top="270" text="Jaká byla atmosféra na jevišti?" backgroundColor="#ff4c00" />
	<label textWrap="true" marginLeft="67" top="320" text="Přemýšlím, že bych šel o víkendu." backgroundColor="#ff4c00" />
	<label textWrap="true" marginLeft="165" top="380" text="Atmosféra byla skvělá!" backgroundColor="#64d13e" />
	<label textWrap="true" marginLeft="113" top="430" text="Hudba tomu hodně pomohla." backgroundColor="#64d13e" />
	<label textWrap="true" marginLeft="203" top="490" text="Tak to už se těším!" backgroundColor="#ff4c00" />
	
	{#each $messages as message, i}
		<label
			left="20"
			top={550 + (i * 50)}
			text={message}
			backgroundColor="#76a8ff"
			marginTop="10"
		/>
	{/each}

	<stackLayout left="0" top="300" width="100%" height="100%" orientation="horizontal">
		<textField left="0" top="620" bind:text={textElem} hint="Type your message here" />
		<button left="0" top="620" text="" on:tap={sendMessage}> </button>
	</stackLayout>
</absoluteLayout>

<style>
	textField {
		width: 245;
		height: 50;
		border-radius: 10;
		padding: 10;
		font-size: 20;
	}

	button {
		background-color: #76a8ff;
		border-radius: 20%;
	}

	label {
		color: #0f0f0f;
		font-size: 20;
		margin: 10;
		padding: 10;
		border-radius: 10%;
	}
</style>
