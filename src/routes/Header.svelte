<script lang="ts">
  import { onMount } from 'svelte';

	import logo from '$lib/images/anchor.png';
	import AirDatepicker from 'air-datepicker';
	import 'air-datepicker/air-datepicker.css';
	import localeEn from 'air-datepicker/locale/en';

	let power: boolean = true;
	let clock: string = "";

	onMount(() => {
		let startDate = new Date();
		new AirDatepicker('#clock', {
			startDate,
			timepicker: true,
			timeFormat: 'h:m aa',
			locale: localeEn,
			position: 'bottom right',
			visible: false
		});
		setInterval(() => {
			clock = new Date().toLocaleTimeString('en-us', { year: "numeric", month: "short", day: "numeric" })
		}, 1000);
	})
</script>

<header>
	<div class="corner">
		<a href="/" on:click={() => power = !power}>
			<img src={logo} alt="SvelteKit" style={power ? null : "filter: invert(1);"}/>
		</a>
	</div>

	<nav>
		<svg viewBox="0 0 2 3" aria-hidden="true">
			<path d="M0,0 L1,2 C1.5,3 1.5,3 2,3 L2,0 Z" />
		</svg>
		<ul>
			<li>
				<a href="//istrav.com">Website</a>
			</li>
			<li>
				<a href="//istrav.live">Live</a>
			</li>
			<li>
				<a href="//istrav.net">Community</a>
			</li>
			<li>
				<a href="//istrav.info">Information</a>
			</li>
			<li>
				<a href="//istrav.pro">Professional</a>
			</li>
		</ul>
		<svg viewBox="0 0 2 3" aria-hidden="true">
			<path d="M0,0 L0,3 C0.5,3 0.5,3 1,2 L2,0 Z" />
		</svg>
	</nav>

	<input type="text" id="clock" value={clock} />
</header>

<style>
	header {
		display: flex;
		justify-content: space-between;
	}

	#clock {
		width: 175px;
		height: 2em;
		margin: 0.5em;
		margin-left: -150px;
		text-align: center;
		border: 2px solid #000;
	}

	.corner {
		width: 3em;
		height: 3em;
	}

	.corner a {
		display: flex;
		align-items: center;
		justify-content: center;
		width: 100%;
		height: 100%;
	}

	.corner img {
		width: 2em;
		height: 2em;
		object-fit: contain;
	}

	nav {
		color: #000;
		font-family: Arial, Helvetica, sans-serif;
		display: flex;
		justify-content: center;
		--background: #fff;
	}

	svg {
		width: 2em;
		height: 3em;
		display: block;
	}

	path {
		fill: var(--background);
	}

	ul {
		position: relative;
		padding: 0;
		margin: 0;
		height: 3em;
		display: flex;
		justify-content: center;
		align-items: center;
		list-style: none;
		background: var(--background);
		background-size: contain;
	}

	li {
		position: relative;
		height: 100%;
	}

	li[aria-current='page']::before {
		--size: 6px;
		content: '';
		width: 0;
		height: 0;
		position: absolute;
		top: 0;
		left: calc(50% - var(--size));
		border: var(--size) solid transparent;
		border-top: var(--size) solid var(--color-theme-1);
	}

	nav a {
		display: flex;
		height: 100%;
		align-items: center;
		padding: 0 0.5rem;
		color: var(--color-text);
		font-weight: 700;
		font-size: 0.8rem;
		text-transform: uppercase;
		letter-spacing: 0.1em;
		text-decoration: none;
		transition: color 0.2s linear;
	}

	a:hover {
		color: var(--color-theme-1);
	}
</style>
