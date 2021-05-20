<script>
	import Footer from '../components/layout/Footer.svelte';

	const macbookSketch = '/img/demo/sketch.png';

	// Team
	const twitterWhite = 'img/logos/twitter-white.svg';
	const twitterBlack = 'img/logos/twitter-black.svg';

	const abitcoinpersonPhoto = '/img/team/abitcoinperson.jpg';
	const dreadPhoto = '/img/team/dread.jpg';
	const elainePhoto = '/img/team/elaine.png';
	const j9RoemPhoto = '/img/team/j9Roem.png';
	const jamesPhoto = '/img/team/james.jpg';
	const k3tanPhoto = '/img/team/k3tan.png';
	const mattOdellPhoto = '/img/team/matt.jpg';
	const niftyneiPhoto = '/img/team/niftynei.jpg';
	const udiPhoto = '/img/team/udi.jpg';

	// Supporters
	const andrewWBlairLogo = '/img/supporters/andrew-w-blair.jpg';
	const thebitcoincompanyLogo = '/img/supporters/thebitcoincompany.jpg';
	const bottlepayLogo = '/img/supporters/bottlepay.png';
	const btcPayServerLogo = '/img/supporters/btc-pay-server.png';
	const duxReserveLogoWithCastlenine = '/img/supporters/castlenine-dux-reserve.jpg';
	const coinkiteLogo = '/img/supporters/coinkite.png';
	const gregFossLogo = '/img/supporters/greg-foss.jpg';
	const jeremyRubinLogo = '/img/supporters/jeremy-rubin.gif';
	const johnPfefferLogo = '/img/supporters/john-pfeffer.jpg';
	const ledgerLogo = '/img/supporters/ledger.jpg';
	const nodlLogo = '/img/supporters/nodl.jpg';
	const silvergateBankLogo = '/img/supporters/silvergate-bank.png';
	const swanBitcoinLogo = '/img/supporters/swan.jpg';
	const ten31Logo = '/img/supporters/ten31.jpg';
</script>

<svelte:head>
	<title>Open Sats | Non-profit aiming to support a sustainable ecosystem of contributors to free and open source software like Bitcoin Core</title>
</svelte:head>

<section class="hero is-medium custom-gradient">
	<div class="hero-body">
		<div class="container">
			<div class="columns is-centered">
				<div class="column is-10 is-12-mobile">
					<h1 class="title is-2 is-family-primary has-text-left has-text-white">Support contributors to Bitcoin and other free and open source projects</h1>
					<br />
					<br />
					<a class="button is-medium is-white button-custom-width" href="/apply">Submit your project</a>
					<p class="is-size-7 has-text-white pt-2">
						If you're a contributor to Bitcoin Core or a related free and open source project, please apply to be pre-listed on our site when we fully launch
						our donation platform.
					</p>
				</div>
			</div>
		</div>
	</div>
</section>

<section class="hero is-medium">
	<div class="hero-body">
		<div class="container">
			<div class="columns">
				<div class="column is-12">
					<h2 class="title is-4 has-text-centered mb-6">Full donation platform coming soon</h2>
					<p class="subtitle is-5 has-text-justified custom-flex mb-6-custom">
						Open Sats is building a web donation platform where donors can learn, donate, and contribute to Bitcoin Core and related free and open source
						projects.
						<br />
						<br />
						We are extremely proud to pass through 100% of charitable donations. Nobody in the organization makes any money. Open Sats will accept donations in both
						bitcoin and fiat currency (credit/debit, wire, etc.) however all donations will be converted to, held, and distributed in bitcoin.
					</p>
					<img src={macbookSketch} alt="Sketch" class="sketch-macbook" title="Teaser" />
					<div class="border-black" />
				</div>
			</div>
			<div class="columns is-centered">
				<div class="column is-8 is-12-mobile">
					<p class="subtitle is-5 has-text-justified">
						Open Sats Initiative, Inc. is a registered non-profit organization (EIN 85-2722249). We have applied for 501(c)(3) status with the IRS and our 1023
						application is currently pending. If we are approved, donations to Open Sats from U.S. taxpayers will be tax-exempt, including donations made during
						our application period.
					</p>
				</div>
			</div>

			<div class="columns mt-6">
				<div class="column is-12">
					<div class="buttons is-centered">
						<a href="/donate" class="button is-primary button-custom-small-width">Donate</a>
						<a href="/contact" class="button is-black button-custom-small-width">Contact us</a>
					</div>
				</div>
			</div>
		</div>
	</div>
</section>

<section class="hero is-medium is-black">
	<div class="hero-body">
		<div class="container">
			<div class="columns is-centered">
				<div class="column is-10 is-12-mobile">
					<h2 class="title is-4 is-family-secondary has-text-centered has-text-white has-text-weight-medium">Board Members</h2>
				</div>
			</div>
		</div>

		<div class="columns is-centered mt-6 custom-width-team-photo">
			<div class="column is-4">
				<img src={j9RoemPhoto} alt="J9Roem" class="team-photo" />
				<p class="has-text-white has-text-centered has-text-weight-semibold mt-5">Janine</p>
				<a href="https://twitter.com/J9Roem" target="_blank"><img src={twitterWhite} alt="Twitter" class="twitter-logo" /></a>
			</div>
			<div class="column is-4">
				<img src={dreadPhoto} alt="Dread" class="team-photo" />
				<p class="has-text-white has-text-centered has-text-weight-semibold mt-5">Dread</p>
				<a href="https://twitter.com/PoleVaultDream" target="_blank"><img src={twitterWhite} alt="Twitter" class="twitter-logo" /></a>
			</div>
			<div class="column is-4">
				<img src={elainePhoto} alt="Elaine" class="team-photo" />
				<p class="has-text-white has-text-centered has-text-weight-semibold mt-5">Elaine Ou</p>
				<a href="https://twitter.com/eiaine" target="_blank"><img src={twitterWhite} alt="Twitter" class="twitter-logo" /></a>
			</div>
		</div>

		<div class="columns is-centered mt-6 custom-width-team-photo">
			<div class="column is-4">
				<img src={jamesPhoto} alt="James" class="team-photo" />
				<p class="has-text-white has-text-centered has-text-weight-semibold mt-5">James O’Beirne</p>
				<a href="https://twitter.com/jamesob" target="_blank"><img src={twitterWhite} alt="Twitter" class="twitter-logo" /></a>
			</div>
			<div class="column is-4">
				<img src={k3tanPhoto} alt="K3tan" class="team-photo" />
				<p class="has-text-white has-text-centered has-text-weight-semibold mt-5">K3tan</p>
				<a href="https://twitter.com/_k3tan" target="_blank"><img src={twitterWhite} alt="Twitter" class="twitter-logo" /></a>
			</div>
			<div class="column is-4">
				<img src={mattOdellPhoto} alt="Matt Odell" class="team-photo" />
				<p class="has-text-white has-text-centered has-text-weight-semibold mt-5">Matt Odell</p>
				<a href="https://twitter.com/matt_odell" target="_blank"><img src={twitterWhite} alt="Twitter" class="twitter-logo" /></a>
			</div>
		</div>

		<div class="columns is-centered mt-6 custom-width-team-photo">
			<div class="column is-4">
				<img src={niftyneiPhoto} alt="Niftynei" class="team-photo" />
				<p class="has-text-white has-text-centered has-text-weight-semibold mt-5">Lisa Neigut</p>
				<a href="https://twitter.com/niftynei" target="_blank"><img src={twitterWhite} alt="Twitter" class="twitter-logo" /></a>
			</div>
			<div class="column is-4">
				<img src={udiPhoto} alt="Udi" class="team-photo" />
				<p class="has-text-white has-text-centered has-text-weight-semibold mt-5">Udi Wertheimer</p>
				<a href="https://twitter.com/udiwertheimer" target="_blank"><img src={twitterWhite} alt="Twitter" class="twitter-logo" /></a>
			</div>
			<div class="column is-4">
				<img src={abitcoinpersonPhoto} alt="Abitcoinperson" class="team-photo" />
				<p class="has-text-white has-text-centered has-text-weight-semibold mt-5">Ben Price</p>
				<a href="https://twitter.com/abitcoinperson" target="_blank"><img src={twitterWhite} alt="Twitter" class="twitter-logo" /></a>
			</div>
		</div>
	</div>
</section>

<section class="hero is-medium">
	<div class="hero-body">
		<div class="container">
			<div class="columns is-centered">
				<div class="column is-12">
					<h2 class="title is-4 is-family-secondary has-text-centered has-text-weight-medium">
						Thanks to our contributors, partners and early supporting organizations for their support, reduced fees, pro-bono services, and free and open source
						tools
					</h2>
					<h4 class="subtitle is-5 is-family-secondary has-text-centered has-text-weight-normal"><a href="/donate">Click here to support Open Sats</a></h4>
				</div>
			</div>

			<!-- Desktop -->
			<div class="columns is-centered mt-6 is-hidden-touch">
				<div class="column is-3">
					<a href="https://bottlepay.com/" target="_blank"><img src={bottlepayLogo} alt="BottlePay logo" class="img-brand" /></a>
					<p class="has-text-centered has-text-weight-semibold mt-5"><a href="https://bottlepay.com/" target="_blank">Bottlepay</a></p>
					<a href="https://twitter.com/bottlepay" target="_blank"><img src={twitterBlack} alt="Twitter" class="twitter-logo" /></a>
				</div>
				<div class="column is-3">
					<a href="https://btcpayserver.org/" target="_blank"><img src={btcPayServerLogo} alt="BTCPay Server logo" class="img-brand" /></a>
					<p class="has-text-centered has-text-weight-semibold mt-5"><a href="https://btcpayserver.org/" target="_blank">BTCPay Server</a></p>
					<a href="https://twitter.com/BtcpayServer" target="_blank"><img src={twitterBlack} alt="Twitter" class="twitter-logo" /></a>
				</div>
				<div class="column is-3">
					<a href="https://twitter.com/castlenine_" target="_blank"
						><img src={duxReserveLogoWithCastlenine} alt="Castlenine - Dux Reserve" class="img-brand" /></a
					>
					<p class="has-text-centered has-text-weight-semibold mt-5">
						Castlenine (<a href="https://twitter.com/duxreserve" target="_blank" class="is-underlined">Dux Reserve</a>)
					</p>
					<a href="https://twitter.com/castlenine_" target="_blank"><img src={twitterBlack} alt="Twitter" class="twitter-logo" /></a>
				</div>
				<div class="column is-3">
					<a href="https://coinkite.com/" target="_blank"><img src={coinkiteLogo} alt="Coinkite logo" class="img-brand" /></a>
					<p class="has-text-centered has-text-weight-semibold mt-5"><a href="https://coinkite.com/" target="_blank">Coinkite</a></p>
					<a href="https://twitter.com/Coinkite" target="_blank"><img src={twitterBlack} alt="Twitter" class="twitter-logo" /></a>
				</div>
			</div>

			<div class="columns is-centered mt-6 is-hidden-touch">
				<div class="column is-3">
					<a href="https://twitter.com/FossGregfoss" target="_blank"><img src={gregFossLogo} alt="Greg Foss" class="img-brand" /></a>
					<p class="has-text-centered has-text-weight-semibold mt-5">Greg Foss</p>
					<a href="https://twitter.com/FossGregfoss" target="_blank"><img src={twitterBlack} alt="Twitter" class="twitter-logo" /></a>
				</div>
				<div class="column is-3">
					<div class="forced-black-box">
						<a href="https://judica.org/" target="_blank"><img src={jeremyRubinLogo} alt="Jeremy Rubin logo" class="img-black-box" /></a>
					</div>
					<p class="has-text-centered has-text-weight-semibold mt-5">
						Jeremy Rubin (<a href="https://judica.org/" target="_blank" class="is-underlined">judica.org</a>)
					</p>
					<a href="https://twitter.com/JeremyRubin" target="_blank"><img src={twitterBlack} alt="Twitter" class="twitter-logo" /></a>
				</div>
				<div class="column is-3">
					<a href="https://twitter.com/jlppfeffer" target="_blank"><img src={johnPfefferLogo} alt="John Pfeffer" class="img-brand" /></a>
					<p class="has-text-centered has-text-weight-semibold mt-5">John Pfeffer</p>
					<a href="https://twitter.com/jlppfeffer" target="_blank"><img src={twitterBlack} alt="Twitter" class="twitter-logo" /></a>
				</div>
				<div class="column is-3">
					<a href="https://www.ledger.com/" target="_blank"><img src={ledgerLogo} alt="Ledger logo" class="img-brand" /></a>
					<p class="has-text-centered has-text-weight-semibold mt-5"><a href="https://www.ledger.com/" target="_blank">Ledger</a></p>
					<a href="https://twitter.com/Ledger" target="_blank"><img src={twitterBlack} alt="Twitter" class="twitter-logo" /></a>
				</div>
			</div>

			<div class="columns is-centered mt-6 is-hidden-touch">
				<div class="column is-3">
					<a href="https://www.nodl.it/" target="_blank"><img src={nodlLogo} alt="Nodl logo" class="img-brand" /></a>
					<p class="has-text-centered has-text-weight-semibold mt-5"><a href="https://www.nodl.it/" target="_blank">nodl</a></p>
					<a href="https://twitter.com/nodl_it" target="_blank"><img src={twitterBlack} alt="Twitter" class="twitter-logo" /></a>
				</div>
				<div class="column is-3">
					<a href="https://silvergate.com/" target="_blank"><img src={silvergateBankLogo} alt="Silvergate Bank logo" class="img-brand" /></a>
					<p class="has-text-centered has-text-weight-semibold mt-5"><a href="https://silvergate.com/" target="_blank">Silvergate Bank</a></p>
					<a href="https://twitter.com/silvergatebank" target="_blank"><img src={twitterBlack} alt="Twitter" class="twitter-logo" /></a>
				</div>
				<div class="column is-3">
					<a href="https://www.swanbitcoin.com/" target="_blank"><img src={swanBitcoinLogo} alt="Swan Bitcoin logo" class="img-brand" /></a>
					<p class="has-text-centered has-text-weight-semibold mt-5"><a href="https://www.swanbitcoin.com/" target="_blank">Swan Bitcoin</a></p>
					<a href="https://twitter.com/SwanBitcoin" target="_blank"><img src={twitterBlack} alt="Twitter" class="twitter-logo" /></a>
				</div>
				<div class="column is-3">
					<a href="https://www.lowtimepreferencefund.com/" target="_blank"><img src={ten31Logo} alt="Ten31 logo" class="img-brand" /></a>
					<p class="has-text-centered has-text-weight-semibold mt-5"><a href="https://www.lowtimepreferencefund.com/" target="_blank">Ten31</a></p>
					<a href="https://twitter.com/Ten31_io" target="_blank"><img src={twitterBlack} alt="Twitter" class="twitter-logo" /></a>
				</div>
			</div>

			<div class="columns is-centered mt-6 is-hidden-touch">
				<div class="column is-3">
					<a href="https://www.manningfulton.com/people/attorneys/andrew-w-blair/" target="_blank"
						><img src={andrewWBlairLogo} alt="Andrew W. Blair" class="img-brand" /></a
					>
					<p class="has-text-centered has-text-weight-semibold mt-5">
						<a href="https://www.manningfulton.com/people/attorneys/andrew-w-blair/" target="_blank">Andrew W. Blair</a>
					</p>
				</div>
				<div class="column is-3">
					<a href="https://twitter.com/thebtccompany" target="_blank"><img src={thebitcoincompanyLogo} alt="The Bitcoin Company" class="img-brand" /></a>
					<p class="has-text-centered has-text-weight-semibold mt-5"><a href="" target="_blank">The Bitcoin Company</a></p>
					<a href="https://twitter.com/thebtccompany" target="_blank"><img src={twitterBlack} alt="Twitter" class="twitter-logo" /></a>
				</div>
			</div>

			<!-- Mobile -->
			<div class="columns is-centered mt-3 is-hidden-desktop">
				<div class="column is-6">
					<a href="https://bottlepay.com/" target="_blank"><img src={bottlepayLogo} alt="BottlePay logo" class="img-brand" /></a>
					<p class="has-text-centered has-text-weight-semibold mt-5"><a href="https://bottlepay.com/" target="_blank">Bottlepay</a></p>
					<a href="https://twitter.com/bottlepay" target="_blank"><img src={twitterBlack} alt="Twitter" class="twitter-logo" /></a>
				</div>
				<div class="column is-6">
					<a href="https://btcpayserver.org/" target="_blank"><img src={btcPayServerLogo} alt="BTCPay Server logo" class="img-brand" /></a>
					<p class="has-text-centered has-text-weight-semibold mt-5"><a href="https://btcpayserver.org/" target="_blank">BTCPay Server</a></p>
					<a href="https://twitter.com/BtcpayServer" target="_blank"><img src={twitterBlack} alt="Twitter" class="twitter-logo" /></a>
				</div>
			</div>

			<div class="columns is-centered is-hidden-desktop">
				<div class="column is-6">
					<a href="https://twitter.com/castlenine_" target="_blank"
						><img src={duxReserveLogoWithCastlenine} alt="Castlenine - Dux Reserve" class="img-brand" /></a
					>
					<p class="has-text-centered has-text-weight-semibold mt-5">
						Castlenine (<a href="https://twitter.com/duxreserve" target="_blank" class="is-underlined">Dux Reserve</a>)
					</p>
					<a href="https://twitter.com/castlenine_" target="_blank"><img src={twitterBlack} alt="Twitter" class="twitter-logo" /></a>
				</div>
				<div class="column is-6">
					<a href="https://coinkite.com/" target="_blank"><img src={coinkiteLogo} alt="Coinkite logo" class="img-brand" /></a>
					<p class="has-text-centered has-text-weight-semibold mt-5"><a href="https://coinkite.com/" target="_blank">Coinkite</a></p>
					<a href="https://twitter.com/Coinkite" target="_blank"><img src={twitterBlack} alt="Twitter" class="twitter-logo" /></a>
				</div>
			</div>

			<div class="columns is-centered is-hidden-desktop">
				<div class="column is-6">
					<a href="https://twitter.com/FossGregfoss" target="_blank"><img src={gregFossLogo} alt="Greg Foss" class="img-brand" /></a>
					<p class="has-text-centered has-text-weight-semibold mt-5">Greg Foss</p>
					<a href="https://twitter.com/FossGregfoss" target="_blank"><img src={twitterBlack} alt="Twitter" class="twitter-logo" /></a>
				</div>
				<div class="column is-6">
					<div class="forced-black-box">
						<a href="https://judica.org/" target="_blank"><img src={jeremyRubinLogo} alt="Jeremy Rubin logo" class="img-black-box" /></a>
					</div>
					<p class="has-text-centered has-text-weight-semibold mt-5">
						Jeremy Rubin (<a href="https://judica.org/" target="_blank" class="is-underlined">judica.org</a>)
					</p>
					<a href="https://twitter.com/JeremyRubin" target="_blank"><img src={twitterBlack} alt="Twitter" class="twitter-logo" /></a>
				</div>
			</div>

			<div class="columns is-centered is-hidden-desktop">
				<div class="column is-6">
					<a href="https://twitter.com/jlppfeffer" target="_blank"><img src={johnPfefferLogo} alt="John Pfeffer" class="img-brand" /></a>
					<p class="has-text-centered has-text-weight-semibold mt-5">John Pfeffer</p>
					<a href="https://twitter.com/jlppfeffer" target="_blank"><img src={twitterBlack} alt="Twitter" class="twitter-logo" /></a>
				</div>
				<div class="column is-6">
					<a href="https://www.ledger.com/" target="_blank"><img src={ledgerLogo} alt="Ledger logo" class="img-brand" /></a>
					<p class="has-text-centered has-text-weight-semibold mt-5"><a href="https://www.ledger.com/" target="_blank">Ledger</a></p>
					<a href="https://twitter.com/Ledger" target="_blank"><img src={twitterBlack} alt="Twitter" class="twitter-logo" /></a>
				</div>
			</div>

			<div class="columns is-centered is-hidden-desktop">
				<div class="column is-6">
					<a href="https://www.nodl.it/" target="_blank"><img src={nodlLogo} alt="Nodl logo" class="img-brand" /></a>
					<p class="has-text-centered has-text-weight-semibold mt-5"><a href="https://www.nodl.it/" target="_blank">nodl</a></p>
					<a href="https://twitter.com/nodl_it" target="_blank"><img src={twitterBlack} alt="Twitter" class="twitter-logo" /></a>
				</div>
				<div class="column is-6">
					<a href="https://silvergate.com/" target="_blank"><img src={silvergateBankLogo} alt="Silvergate Bank logo" class="img-brand" /></a>
					<p class="has-text-centered has-text-weight-semibold mt-5"><a href="https://silvergate.com/" target="_blank">Silvergate Bank</a></p>
					<a href="https://twitter.com/silvergatebank" target="_blank"><img src={twitterBlack} alt="Twitter" class="twitter-logo" /></a>
				</div>
			</div>

			<div class="columns is-centered is-hidden-desktop">
				<div class="column is-6">
					<a href="https://www.swanbitcoin.com/" target="_blank"><img src={swanBitcoinLogo} alt="Swan Bitcoin logo" class="img-brand" /></a>
					<p class="has-text-centered has-text-weight-semibold mt-5"><a href="https://www.swanbitcoin.com/" target="_blank">Swan Bitcoin</a></p>
					<a href="https://twitter.com/SwanBitcoin" target="_blank"><img src={twitterBlack} alt="Twitter" class="twitter-logo" /></a>
				</div>
				<div class="column is-6">
					<a href="https://www.lowtimepreferencefund.com/" target="_blank"><img src={ten31Logo} alt="Ten31 logo" class="img-brand" /></a>
					<p class="has-text-centered has-text-weight-semibold mt-5"><a href="https://www.lowtimepreferencefund.com/" target="_blank">Ten31</a></p>
					<a href="https://twitter.com/Ten31_io" target="_blank"><img src={twitterBlack} alt="Twitter" class="twitter-logo" /></a>
				</div>
			</div>

			<div class="columns is-centered is-hidden-desktop">
				<div class="column is-6">
					<a href="https://www.manningfulton.com/people/attorneys/andrew-w-blair/" target="_blank"
						><img src={andrewWBlairLogo} alt="Andrew W. Blair" class="img-brand" /></a
					>
					<p class="has-text-centered has-text-weight-semibold mt-5">
						<a href="https://www.manningfulton.com/people/attorneys/andrew-w-blair/" target="_blank">Andrew W. Blair</a>
					</p>
				</div>
				<div class="column is-6">
					<a href="https://twitter.com/thebtccompany" target="_blank"><img src={thebitcoincompanyLogo} alt="The Bitcoin Company" class="img-brand" /></a>
					<p class="has-text-centered has-text-weight-semibold mt-5"><a href="" target="_blank">The Bitcoin Company</a></p>
					<a href="https://twitter.com/thebtccompany" target="_blank"><img src={twitterBlack} alt="Twitter" class="twitter-logo" /></a>
				</div>
			</div>
		</div>
	</div>
</section>

<Footer />

<style lang="scss">
	.sketch-macbook {
		display: block;
		max-width: 720px !important;
		height: auto !important;
		margin: 1rem auto 4rem !important;
		text-align: center;
	}

	.custom-flex {
		display: flex;
		justify-content: center;
		width: 66.66667%;
		margin-right: auto;
		margin-left: auto;
	}

	.custom-gradient {
		background: rgb(233, 93, 28);
		background: radial-gradient(circle, rgba(233, 93, 28, 1) 4%, rgba(233, 62, 28, 1) 61%, rgba(233, 31, 28, 1) 100%);
	}

	.is-underlined {
		text-decoration: underline;
	}

	.button-custom-small-width {
		min-width: 125px;
	}

	.button-custom-width {
		min-width: 150px;
	}

	.img-brand {
		display: block;
		width: 80%;
		max-width: 300px;
		height: auto;
		margin-right: auto;
		margin-left: auto;
		box-shadow: 0 0 0 2px #000000;
	}

	.mb-6-custom {
		margin-bottom: 5rem;
	}

	.img-black-box {
		width: 100%;
		height: auto;
	}

	.forced-black-box {
		display: flex;
		justify-content: center;
		align-items: center;
		width: 80%;
		max-width: 300px;
		height: 74%;
		margin-right: auto;
		margin-left: auto;
		box-shadow: 0 0 0 2px #000000;
		background-color: #000000;
	}

	.custom-width-team-photo {
		max-width: 1000px;
		margin-right: auto;
		margin-left: auto;
	}

	.team-photo {
		display: block;
		width: 80%;
		max-width: 242px;
		height: auto;
		margin-right: auto;
		margin-left: auto;
		box-shadow: 0 0 0 2px #ffffff;
	}

	.twitter-logo {
		display: block;
		width: 22px;
		height: auto;
		margin-top: 10px;
		margin-right: auto;
		margin-left: auto;
	}

	.border-black {
		width: 400px;
		height: 2px;
		margin: 8rem auto;
		background-color: #000000;
	}

	@media screen and (max-width: 385px) {
		.border-black {
			width: 222px;
		}
	}

	@media screen and (min-width: 386px) and (max-width: 445px) {
		.border-black {
			width: 282px;
		}
	}

	@media screen and (min-width: 446px) and (max-width: 480px) {
		.border-black {
			width: 342px;
		}
	}

	@media screen and (max-width: 768px) {
		.sketch-macbook {
			width: 420px !important;
			max-width: 100% !important;
		}

		.custom-flex {
			display: flex;
			justify-content: center;
			width: 88.88889%;
			margin-right: auto;
			margin-left: auto;
		}
	}

	@media screen and (max-width: 1023px) {
		.forced-black-box {
			margin-top: 1.5rem;
		}

		.img-brand {
			margin-top: 1.5rem;
		}
	}
</style>
