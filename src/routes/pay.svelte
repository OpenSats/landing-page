<svelte:head>
	<title>Open Sats | Donation bitcoin payment</title>
</svelte:head>

<section class="hero is-medium ">
	<div class="hero-body">
		<div class="container">
			<div class="columns is-centered mb-6">
				<div class="column is-11 is-12-mobile">
					<h1 class="title is-4 is-family-primary has-text-centered">
						To donate bitcoin, please enter the dollar amount, invoice number, and email address associated with the invoice you received via email.
					</h1>
					<h2 class="title is-4 is-family-primary has-text-centered">This will generate a BTCPay Server invoice which you can then pay.</h2>
				</div>
			</div>
			<div class="columns is-centered mt-3">
				<div class="column is-6 is-6-desktop is-8-tablet is-10-mobile is-offset-1-mobile">
					<form method="POST" action="https://donate.opensats.org/btcqbo/verify">
						<div class="field">
							<label class="label" for="amount">USD Amount</label>
							<div class="control">
								<input class="input" type="number" name="amount" id="amount" min="0" step="0.01" />
							</div>
						</div>

						<div class="field">
							<label class="label" for="email">Email Address</label>
							<div class="control">
								<input class="input" type="email" name="email" id="email" />
							</div>
						</div>

						<div class="field">
							<label class="label" for="orderId">Invoice Number</label>
							<div class="control">
								<input class="input" type="text" name="orderId" id="orderId" />
							</div>
						</div>

						<input type="hidden" name="notificationUrl" value="https://donate.opensats.org/btcqbo/api/v1/payment" />
						<input type="hidden" name="redirectUrl" value="https://opensats.org" />

						<div class="buttons is-centered mt-6">
							<button class="button is-primary" type="submit">Pay with bitcoin</button>
						</div>
					</form>
				</div>
			</div>
		</div>
	</div>
</section>
