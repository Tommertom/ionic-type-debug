<ion-card>
	<ion-card-header>
		<ion-card-subtitle>Great success!!</ion-card-subtitle>
		<ion-card-title>Welcome to your app!</ion-card-title>
	</ion-card-header>

	<ion-card-content>
		<ion-grid>
			<ion-row>
				<ion-col>1</ion-col>
				<ion-col>2</ion-col>
				<ion-col size="'3'">3</ion-col>

				<ion-col>5</ion-col>
				<ion-col>6</ion-col>
			</ion-row>
		</ion-grid>

		Thank you for using this starter. Click buttons below to open these guides (will open in new
		window). Don't forget to open DevTools to see this app in mobile mode. Happy coding!!!
	</ion-card-content>
	<ion-button hidden={false} target="_new" fill="outline" slot="end">View</ion-button>
	<ion-item>
		<ion-label>Visit Ionic Showcase app with sourceviewer</ion-label>
		<ion-button href="https://ionicsvelte.firebaseapp.com/" target="_new" fill="outline" slot="end"
			>View</ion-button
		>
	</ion-item>

	<ion-item>
		<ion-label>Visit Ionic component docs</ion-label>
		<ion-button
			href="https://ionicframework.com/docs/components"
			target="_new"
			draggable={false}
			fill="default"
			slot="end">View</ion-button
		>
	</ion-item>
	<div on:click={console.log} on:keydown={console.log}>sads</div>
	<ion-item>
		<ion-label>Visit Svelte Kit docs</ion-label>
		<ion-button
			href="https://kit.svelte.dev/docs/introduction"
			on:ionBlur={console.log}
			on:copy={console.log}
			target="_new"
			class="asd"
			fill="outline"
			slot="end">View</ion-button
		>
	</ion-item>
	<ion-item>
		<ion-label>Visit Svelte docs</ion-label>
		<ion-button href="https://svelte.dev/docs" target="_new" fill="outline" slot="end"
			>View</ion-button
		>
	</ion-item>
</ion-card>
