# Typings debug project
Project to debug Ionic typings for Svelte

See typings file in `node_modules/ionic-svelte/index.d.ts`

tsconfig.json
```
{
	"extends": "./.svelte-kit/tsconfig.json",
	"compilerOptions": {
		"typeRoots": [
			"./node_modules/ionic-svelte"
		],
		"types": [
			"ionic-svelte"
		],
		"allowJs": true,
		"checkJs": true,
		"esModuleInterop": true,
		"forceConsistentCasingInFileNames": true,
		"resolveJsonModule": true,
		"skipLibCheck": true,
		"sourceMap": true,
		"strict": true
	}
	// Path aliases are handled by https://kit.svelte.dev/docs/configuration#alias
	//
	// If you want to overwrite includes/excludes, make sure to copy over the relevant includes/excludes
	// from the referenced tsconfig.json - TypeScript does not merge them in
}

```

N.B.
`node_modules/ionic-svelte/package.json` has ` "types": "index.d.ts",` in it. Not sure if that actually replaces the `tsconfig.json` part in order to include the typings? (I saw this in some other package).


~~## known issue - high severity (SHOULD BE CLOSED?)~~

Some attributes give same error. See `+page.svelte` in `routes`.
```
Argument of type '{ ****: string; }' is not assignable to parameter of type 'HTMLBaseAttributes | Ion***'.
  Type '{ ****: string; }' is missing the following properties from type 'Ion***Col***': addEventListener, dispatchEvent, removeEventListenerjs(2345)
```

```
<ion-col size="'3'">3</ion-col>
<ion-accordion value="colors">
<ion-list inset={true}>
<ion-breadcrumbs max-items={4}>
<ion-breadcrumb href="#">
```

## known issue - low severity
Empty interface declaration needed in order to get typescript errors in vscode for default HTML attributes/events

```
export interface HTMLBaseAttributes extends HTMLAttributes<HTMLBaseElement> {
}
```

So we do

```
'ion-button': IonButton | HTMLBaseAttributes;
```

instead of

```
 'ion-button': IonButton | HTMLAttributes<HTMLBaseElement>;
```

Can this be done without an empty interface?
