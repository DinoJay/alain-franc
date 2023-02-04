<script>
	import { fade } from 'svelte/transition';

	let visible = null;

	setTimeout(() => {
		visible = true;
	}, 7300);
</script>

<div
	class="bg-cover bg h-screen w-screen"
	style="{`background-image: url(/gif_E.webp); transform: rotate(-0deg) `} "
>
	{#if visible}
		<div class="w-full h-full bg-white text" transition:fade>
			Ils font tutu-panpan à l'automne et emménagent au pringtemps suivant. Ils rénovent une maison
			de vacances et s'échangent leurs promesses. Ensemble ils vont se dire Oui ! Alain + François
			se marient. Ils ont le plaisir de vous accueillir sous le thème de la folie et de l'élégance
			tropicale Le 15 juillet 2023 à 16h R. Conselheiro Dr. Antero P. Leitão 13, 3060-082, Portugal
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
		animation-duration: 6s;
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
			background-image: url(/gif_A.webp);
			transform: scale(1) rotate(0deg);
		}

		25% {
			background-image: url(/gif_B.webp);
			transform: scale(1.2) rotate(25deg);
		}

		50% {
			background-image: url(/gif_C.webp);
			transform: scale(1) rotate(50deg);
		}

		75% {
			background-image: url(/gif_D.webp);
			transform: scale(1.2) rotate(-25deg);
		}
		100% {
			background-image: url(/gif_E.webp);
			transform: scale(1) rotate(0deg);
			/* content: 'babababa'; */
		}
	}
</style>
