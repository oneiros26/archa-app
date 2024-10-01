<script>
	import { writable } from 'svelte/store';
	let textElem = ''; // Message input
	let messages = writable([]); // Array to store the messages

	function sendMessage() {
		if (textElem) {
			// Add the new message to the messages array
			messages.update((msgs) => [...msgs, textElem]);
			console.log(textElem); // Log the entered message
			textElem = ''; // Clear the input after sending
		}
	}
</script>

<absoluteLayout>
	<label left="110" top="0" text="Hi, want to get some bitches?" backgroundColor="#64d13e" />
	<label left="123" top="50" text="This is the messaging page." backgroundColor="#64d13e" />
	
	<!-- This block dynamically generates new labels for each message -->
	{#each $messages as message, i}
		<label
			right="0"
			top={100 + (i * 50)}
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
	}

	label {
		color: #0f0f0f;
		font-size: 20;
		margin: 10;
		padding: 10;
		border-radius: 10%;
	}
</style>
