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

				<ion-col id="22">5</ion-col>
				<ion-col>6</ion-col>
			</ion-row>
		</ion-grid>

		Thank you for using this starter. Click buttons below to open these guides (will open in new
		window). Don't forget to open DevTools to see this app in mobile mode. Happy coding!!!

		<ion-accordion-group multiple={true} id="multiple">
			<ion-accordion value="colors">
				<ion-item slot="header">
					<ion-label>Colors</ion-label>
				</ion-item>

				<ion-list slot="content">
					<ion-item>
						<ion-label>Red</ion-label>
					</ion-item>
					<ion-item>
						<ion-label>Green</ion-label>
					</ion-item>
					<ion-item>
						<ion-label>Blue</ion-label>
					</ion-item>
				</ion-list>
			</ion-accordion>
		</ion-accordion-group>

		<ion-list inset={true}>
			<ion-list-header>Max Items</ion-list-header>
			<ion-breadcrumbs max-items={4}>
				<ion-breadcrumb href="#"> Home </ion-breadcrumb>
				<ion-breadcrumb href="#electronics"> Electronics </ion-breadcrumb>
				<ion-breadcrumb href="#photography"> Photography </ion-breadcrumb>
				<ion-breadcrumb href="#cameras"> Cameras </ion-breadcrumb>
				<ion-breadcrumb href="#film"> Film </ion-breadcrumb>
				<ion-breadcrumb> 35 mm </ion-breadcrumb>
			</ion-breadcrumbs>
		</ion-list>
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
			href="ssdsd"
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
