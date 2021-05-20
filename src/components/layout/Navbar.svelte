<script>
	import { createEventDispatcher } from 'svelte';
	import { fade, slide } from 'svelte/transition';

	const brandLogo = '/img/logos/logo.png';
	const githubLogo = '/img/logos/github.svg';
	const twitterLogo = '/img/logos/twitter.svg';
	const telegramLogo = '/img/logos/telegram.svg';
	const linkedinLogo = '/img/logos/linkedin.svg';
	const Close = '/img/icons/close.svg';

	const dispatch = createEventDispatcher();

	let scrollPositionY = 0;
	let withBlackBorder = false;

	let showMobileMenu = false;

	const handleShowMobileMenu = () => {
		dispatch('menuOpen');
		showMobileMenu = true;
	};

	const handleCloseMobileMenu = () => {
		dispatch('menuClose');
		showMobileMenu = false;
	};

	const handleCloseMobileMenuLink = () => {
		setTimeout(() => {
			handleCloseMobileMenu();
		}, 121);
	};

	$: if (scrollPositionY > 2) {
		withBlackBorder = true;
	} else {
		withBlackBorder = false;
	}
</script>

<svelte:window bind:scrollY={scrollPositionY} />

<div class="container">
	<nav class="navbar is-fixed-top is-white" class:navbar-black-border={withBlackBorder} role="navigation" aria-label="main navigation">
		<div class="navbar-brand">
			<a class="navbar-item is-hidden-tablet-only is-hidden-mobile-only is-hidden-touch" href="/" title="Vires in Numeris"
				><img src={brandLogo} alt="Open Sats" class="brand-logo" /></a
			>

			<a class="navbar-item is-hidden-desktop" href="/" title="Vires in Numeris"> <img src={brandLogo} alt="Open Sats" class="brand-logo" /></a>

			{#if !showMobileMenu}
				<span
					role="button"
					class="navbar-burger burger"
					aria-label="menu"
					aria-expanded="false"
					data-target="navbar"
					on:click={handleShowMobileMenu}
					transition:fade={{ duration: 800 }}
				>
					<span aria-hidden="true" />
					<span aria-hidden="true" />
					<span aria-hidden="true" />
				</span>
			{/if}
		</div>

		<div id="navbar" class="navbar-menu">
			<div class="navbar-end">
				<a class="navbar-item mr-4" href="/donate">Donate</a>
				<a class="navbar-item mr-4" href="/white-paper" title="Bitcoin Whitepaper">Whitepaper</a>
				<a class="navbar-item mr-4" href="/contact">Contact</a>
				<a class="navbar-item" href="https://twitter.com/opensats" target="_blank" title="Follow us on Twitter">
					<img src={twitterLogo} height="24px" width="24px" alt="Twitter" class="media-logo" />
				</a>
				<a class="navbar-item" href="https://t.me/opensats" target="_blank" title="Join our Telegram">
					<img src={telegramLogo} height="24px" width="24px" alt="Telegram" class="media-logo" />
				</a>
				<a class="navbar-item" href="https://github.com/Open-Sats" target="_blank" title="Don't trust, verify our code">
					<img src={githubLogo} height="24px" width="24px" alt="Github" class="media-logo" />
				</a>
				<a class="navbar-item" href="https://www.linkedin.com/company/opensats" target="_blank" title="Join our Telegram">
					<img src={linkedinLogo} height="24px" width="24px" alt="Linkedin" class="media-logo" />
				</a>
			</div>
		</div>
	</nav>
</div>

{#if showMobileMenu}
	<div class="mobile-menu-overlay" transition:slide={{ duration: 500 }}>
		<div class="mobile-menu-content" transition:fade={{ duration: 222 }}>
			<a href="/" on:click={handleCloseMobileMenuLink}><img class="brand-logo is-unselectable" src={brandLogo} title="Vires in Numeris" /></a>
			<span class="icon is-large is-primary" on:click={handleCloseMobileMenu} transition:fade={{ duration: 444 }}><img src={Close} alt="close" /></span>
			<a class="navbar-item has-text-weight-semibold is-size-5 mt-5" href="/donate" on:click={handleCloseMobileMenuLink}>Donate</a>
			<a class="navbar-item has-text-weight-semibold is-size-5" href="/white-paper" title="Bitcoin Whitepaper" on:click={handleCloseMobileMenuLink}
				>Whitepaper</a
			>
			<a class="navbar-item has-text-weight-semibold is-size-5" href="/contact" on:click={handleCloseMobileMenuLink}>Contact</a>
		</div>
		<div class="social-icons">
			<a href="https://twitter.com/opensats" target="_blank" title="Follow us on Twitter">
				<img src={twitterLogo} height="24px" width="24px" alt="Twitter" class="media-logo" />
			</a>
			<a href="https://t.me/opensats" target="_blank" title="Join our Telegram">
				<img src={telegramLogo} height="24px" width="24px" alt="Telegram" class="media-logo" />
			</a>
			<a href="https://github.com/Open-Sats" target="_blank" title="Don't trust, verify our code">
				<img src={githubLogo} height="24px" width="24px" alt="Github" class="media-logo" />
			</a>
			<a href="https://www.linkedin.com/company/opensats" target="_blank" title="Join our Telegram">
				<img src={linkedinLogo} height="24px" width="24px" alt="Linkedin" class="media-logo" />
			</a>
		</div>
	</div>
{/if}

<style lang="scss">
	.navbar {
		padding-right: 32px;
		padding-left: 32px;
		// Remove tap highlight just for the navbar & the footer
		-webkit-tap-highlight-color: transparent;
	}

	.mt-5 {
		margin-top: 1.75rem !important;
	}

	.brand-logo {
		width: auto;
		height: 20px;
		margin-left: 3px;
	}

	.media-logo {
		width: 24px;
		height: auto;
	}

	.navbar-black-border {
		border-bottom: 1px #000000 solid;
	}

	@media screen and (max-width: 768px) {
		.navbar-burger {
			position: absolute;
			top: 0;
			right: 3px;
			-webkit-tap-highlight-color: rgba(255, 255, 255, 0);
		}
	}

	.mobile-menu-overlay {
		position: fixed;
		top: 0;
		right: 0;
		bottom: 0;
		left: 0;
		z-index: 100;
		height: 110vh;
		box-shadow: 0 10px 30px 2px rgba(18, 39, 120, 0.121);
		background-color: #ffffff;

		.icon {
			position: absolute;
			top: 30px;
			right: 62px;

			img {
				width: 26px;
				margin-bottom: 0.8rem;
				margin-left: 0.4rem;
			}

			&:hover {
				cursor: pointer;
			}
		}

		.is-size-6 {
			-webkit-tap-highlight-color: rgba(255, 255, 255, 0);
		}

		.brand-logo {
			margin-left: 12px;
		}

		.navbar-item {
			margin-bottom: 1.21rem;
		}

		.mobile-menu-content {
			min-height: calc(62vh - 69px);
			padding: 2rem 2.25rem;
		}

		.social-icons {
			display: flex;
			justify-content: center;
			align-items: center;
			margin-top: 1.21rem;
			margin-bottom: 1rem;

			a {
				padding: 0.5rem 0.75rem;
				line-height: 1.5;
			}
		}
	}
</style>
