<script>
	import { Button, TextField } from '@nativescript/core';

	// Click button, read textfield, send message
	Button.on('tap', () => {
        const textField = TextField;
        // get the message from the text field
        const message = textField.text;
        // add new message to the chat
    });
</script>

<absoluteLayout>
	<label left="0" top="0" text="Hi, want to get some bitches?" backgroundColor="#64d13e" />
	<label left="0" top="50" text="This is the messaging page." backgroundColor="#64d13e" />
	<label
		left="50"
		top="100"
		text="You can send messages here."
		backgroundColor="#76a8ff"
		marginTop="30"
	/>
	<label
		left="30"
		top="150"
		text="You can also receive messages."
		backgroundColor="#76a8ff"
        marginTop="30"
        />
    <label
        left="0"
        top="200"
        text="What a nice conversation."
        backgroundColor="#64d13e"
        marginTop="50"
    />
    <label
        left="212"
        top="250"
        text="Skibidi rizz."
        backgroundColor="#76a8ff"
        marginTop="70"
    />

	<stackLayout left="0" top="300" width="100%" height="100%" orientation="horizontal">
		<textField left="0" top="620" hint="Type your message here" />
		<button left="0" top="620" text=""> </button>
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
