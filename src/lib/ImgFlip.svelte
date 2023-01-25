<div class="bg-cover" />

<style>
	div {
		width: 800px;
		height: 667px;
		animation: photos 6s infinite;
		background-repeat: no-repeat;
		/* animation-timing-function: ease-out; */
	}

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
			background-image: url(/gif01_low.webp);
			transform: scale(1) rotate(100deg);
		}

		25% {
			background-image: url(/gif02_low.webp);
			transform: scale(1.2) rotate(25deg);
		}

		50% {
			background-image: url(/gif03_low.webp);
			transform: scale(1) rotate(50deg);
		}

		75% {
			background-image: url(/gif04_low.webp);
			transform: scale(1.2) rotate(75deg);
		}
		100% {
			background-image: url(/gif01_low.webp);
			transform: scale(1) rotate(100deg);
		}
	}
</style>
