<script>
import store from "../store/store";
export default {
	components: {},

	data() {
		return {
			// polaceholder
			store,
		};
	},
	methods: {
		// palceholdewr
	},
	created() {
		// polaceholder
	},
	mounted() {
		// polaceholder
	},
};
</script>

<template>
	<div v-if="store.existData" id="lavora">
		<div class="container-fluid deb mt-5 pb-3">
			<h1 class="text-center pt-5 fw-bold display-5 myColor">LAVORA CON NOI</h1>

			<div class="section_container d-flex">
				<div class="section_left">
					<div class="img_container">
						<img src="https://www.blinkco.io/wp-content/uploads/2021/05/food-delivery_featured-image.jpeg" alt="" />
					</div>
				</div>

				<div class="section_right debug">
					<h1 class="myColor">Unisciti al nostro Team!</h1>
					<p>Diventa un rider e inizia a guadagnare con flessibilità!</p>
					<h5>
						Stai cercando un lavoro flessibile che si adatti ai tuoi orari? Con DeliveBoo, puoi lavorare quando vuoi e guadagnare
						consegnando cibo nella tua città. Unisciti a noi e inizia a fare la differenza, una consegna alla volta!
					</h5>
					<button type="button" class="btn position-relative fw-bold" id="myBtn">
						<div class="background"></div>
						<i class="fa-solid fa-person-biking fs-5 me-1"></i>
						DIVENTA UN RIDER
					</button>
				</div>
			</div>
		</div>
	</div>
</template>

<style scoped>
.myColor {
	color: #912731;
}

#lavora {
	margin-top: 8rem;
	margin-bottom: 6rem;
}

.section_left {
	width: 60%;
	display: flex;
	justify-content: center;
	align-items: center;
}

.img_container {
	width: 90%;
	aspect-ratio: 1.1;
	overflow: hidden;
	border-radius: 30px;
}

img {
	width: 140%;
	margin: 0 -20%;
}

.section_right {
	width: 40%;
	padding: 3rem 1rem;
}

.section_right > * {
	padding: 1rem 0;
}

.section_container {
	margin: 3rem 0;
}

h1 {
	font-weight: 700;
}

.container-fluid {
	margin: auto;
	margin-top: 10rem;
	border-radius: 30px;
	width: 90%;
	-webkit-box-shadow: 0px 0px 50px -4px rgba(0, 0, 0, 0.5);
	box-shadow: 0px 0px 50px -4px rgba(0, 0, 0, 0.5);
	background: white;
}

#myBtn {
	color: white;
	z-index: 2;
	overflow: hidden;
	border: 5px solid transparent;
	background-color: #912731;

	padding: 0.8rem;
}

#myBtn:hover {
	color: #912731;
	border-color: transparent;
}

.background {
	width: 0;
	height: 0;
	position: absolute;
	top: 50%;
	left: 50%;
	transform: translate(-50%, -50%);
	background-color: white;
	transition: 0.4s;
	z-index: -1;
	border: none;
}

button:hover .background {
	width: 150%;
	height: 150%;
}
</style>

<style scoped>
@media (min-width: 1451px) {
	#lavora {
		padding-top: 4rem;
	}
}

@media (max-width: 1000px) {
	.section_left {
		width: 100%;
	}

	.section_right {
		width: 100%;
	}

	.section_container {
		display: flex;
		flex-direction: column;
	}
}
</style>