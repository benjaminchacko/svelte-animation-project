<script>
	let isHidden = true;
</script>

<main>
	<h1>Svelte Animation Project</h1>

	<button on:click={() => (isHidden = !isHidden)}>
		{#if isHidden}Show Text{:else}Hide Text{/if}
	</button>
	{#if !isHidden}
		<div>
			<p>
				Gingerbread jujubes fruitcake lollipop. Halvah cotton candy
				muffin jelly-o. Jelly beans soufflé chocolate bar bear claw
				fruitcake biscuit lemon drops apple pie. Pastry caramels halvah
				donut. Sesame snaps cheesecake jelly-o cheesecake bonbon. Dragée
				gingerbread sweet apple pie topping gummies halvah powder
				tootsie roll. Oat cake cookie pastry croissant. Marshmallow
				topping lollipop. Pie fruitcake liquorice soufflé cake sesame
				snaps macaroon. Dragée donut sesame snaps fruitcake jelly-o
				gummi bears pie. Biscuit bonbon danish cotton candy wafer icing
				pie. Jelly pudding cake dragée brownie pudding soufflé. Icing
				sweet sweet roll chocolate bar powder. Cake caramels cake icing.
				Jelly beans toffee chocolate cake cake. Icing gummi bears donut
				cookie ice cream.
			</p>
			<p>
				Icing cake muffin wafer. Macaroon chupa chups bear claw.
				Macaroon tootsie roll biscuit pie dessert jelly-o. Cupcake ice
				cream powder biscuit danish gingerbread pudding macaroon.
				Dessert sweet roll lollipop marshmallow. Biscuit soufflé biscuit
				chocolate tootsie roll lemon drops muffin macaroon donut. Icing
				carrot cake topping toffee caramels apple pie sesame snaps.
				Sweet roll ice cream tootsie roll. Carrot cake tiramisu
				marshmallow cookie fruitcake. Sweet apple pie fruitcake pudding
				pudding.
			</p>
		</div>
	{/if}
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>
