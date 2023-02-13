<script>
	import { fade } from 'svelte/transition';

	let visible = null;

	setTimeout(() => {
		visible = true;
	}, 8600);
</script>

<div
	class="bg-contain bg bg-center h-screen w-screen"
	style="{`background-image: url(/A_low.webp); transform: rotate(-0deg) `} "
>
	{#if visible}
		<div class="w-full h-full bg-white text text-center " transition:fade>
			<div class="mb-6">
				<p class="blu">
					Ils font "Tutu-panpan" à l'automne et emménagent ensemble au printemps suivant.
				</p>
				<p class="beige">Fazem "Tchiki boum" no Outono e mudam-se juntos na Primavera seguinte.</p>
			</div>

			<div class="mb-6">
				<p class="blu">Ils rénovent une maison de vacances et rêvent d'y célébrer leur union.</p>
				<p class="beige">
					Eles estão a renovar uma casa de férias e sonham em celebrar a sua união lá.
				</p>
			</div>
			<div class="mb-6">
				<p class="blu">Ensemble ils vont se dire Oui !</p>
				<p class="beige">Juntos eles dirão Sim!</p>
			</div>
			<div class="my-24">
				<h1 class="text-2xl font-bold">Alain + François</h1>
				<p class="mb-3"><span class="blu ">se marient</span> / <span class="beige">casam</span></p>
				<p class="italic">15.07.2023 - 16h00</p>
				<p>
					<a href="https://maps.google.com/?q=40.40436721930026,-8.52993730540731"
						>R. Conselheiro Dr. Antero P. Leitão 13, 3060-082, Portugal</a
					>
				</p>
			</div>
			<div class="mb-6">
				<h2 class="text-xl mb-2">↓</h2>
				<p class="blu">
					Ils ont le plaisir de vous accueillir, sous le thème de l'élégance tropicale
				</p>
				<p class="beige">Têm o prazer de vos convidar, sob o tema da elegância tropical.</p>
			</div>

			<div>
				<p class="blu">
					Deux possibilités d'hébergement : - camping sur place. - hôtel et gîtes dans les environs
					(à définir).
				</p>
				<p class="beige">
					Duas possibilidades de alojamento: - acampamento no local. - hotel o alojamento nas
					proximidades (a definir).
				</p>
			</div>
		</div>
	{/if}
</div>

<style>
	.text {
		@apply p-3;
	}
	.bg {
		max-width: 600px;
		max-height: 800px;
		/* animation: photos 6s infinite; */
		background-repeat: no-repeat;
		animation-delay: 1s;
		animation-name: photos;
		animation-duration: 8s;
		/* animation-iteration-count: 1; */
		/* animation-timing-function: ease-out; */
	}

	/* div::before {
		content: " Ils font tutu-panpan à l'automne et emménagent au pringtemps suivant. Ils rénovent une maison de vacances et s'échangent leurs promesses. Ensemble ils vont se dire Oui ! Alain + François se marient. Ils ont le plaisir de vous accueillir sous le thème de la folie et de l'élégance tropicale Le 15 juillet 2023 à 16h R. Conselheiro Dr. Antero P. Leitão 13, 3060-082, Portugal";
	} */

	/* @keyframes photos {
		0% {
			background-image: url(gif01_low.webp);
		}

		14.285% {
			background-image: url(gif02_low.webp);
		}

		28.571% {
			background-image: url(gif03_low.webp);
		}

		42.857% {
			background-image: url(gif04_low.webp);
		}
		57.142% {
			background-image: url(gif05_low.webp);
		}
		71.428% {
			background-image: url(gif06_low.webp);
		}
		85.714% {
			background-image: url(gif07_low.webp);
		}
		100% {
			background-image: url(gif08_low.webp);
		}
	} */
	@keyframes photos {
		0% {
			background-image: url(/A_low.webp);
			transform: scale(1) rotate(0deg);
		}

		25% {
			background-image: url(/B_low.webp);
			transform: scale(1.5) rotate(-180deg);
		}

		50% {
			background-image: url(/C_low.webp);
			transform: scale(1) rotate(180deg);
		}

		75% {
			background-image: url(/D_low.webp);
			transform: scale(2) rotate(-25deg);
		}
		100% {
			background-image: url(/A_low.webp);
			transform: scale(1) rotate(0deg);
			/* content: 'babababa'; */
		}
	}

	.beige {
		color: rgb(202, 142, 91);
	}
	.blu {
		color: rgb(105, 87, 152);
	}
</style>
