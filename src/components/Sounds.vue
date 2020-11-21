<template>
	<v-container fluid grid-list-lg>
		<v-layout wrap>
			<v-flex xs4 v-for="(sound, index) in sounds" :key="index">
				<v-card v-on:click="play(sound.sound)">
					<v-card-text>
						<v-icon color="yellow" x-large>play_arrow</v-icon>
						<p>{{ sound.title }}</p>
					</v-card-text>
				</v-card>
			</v-flex>
		</v-layout>
	</v-container>
</template>

<script>
export default {
	name: 'Sounds',
	data () {
		return {
			sounds: [
				{
					title: "Cow",
					sound: "cow.mp3"
				},
				{
					title: "Bell",
					sound: "bell.mp3"
				},
				{
					title: "Explosion",
					sound: "explosion.mp3"
				},
				{
					title: "Ambulance",
					sound: "ambulance.mp3"
				},
				{
					title: "Bullet",
					sound: "bullet.mp3"
				},
				{
					title: "Fizzle",
					sound: "fizzle.mp3"
				},
				{
					title: "Movie",
					sound: "movie.mp3"
				},
				{
					title: "Punch",
					sound: "punch.mp3"
				},
				{
					title: "Telephone",
					sound: "telephone.mp3"
				},
				{
					title: "Bathroom",
					sound: "bathroom.mp3"
				},
				{
					title: "Banana",
					sound: "Banana.mp3"
				},
				{
					title: "Crocodile",
					sound: "Crocodile.mp3"
				},
				{
					title: "Monkey",
					sound: "Monkey.mp3"
				},
				{
					title: "Elephant",
					sound: "Elephant.mp3"
				},
				{
					title: "Lion",
					sound: "Lion.mp3"
				},
				{
					title: "Tiger",
					sound: "Tiger.mp3"
				},
				{
					title: "Toilet",
					sound: "Toilet.mp3"
				},
				{
					title: "Zebra",
					sound: "Zebra.mp3"
				},
				{
					title: "Giraffe",
					sound: "Giraffe.mp3"
				},
				{
					title: "Camel",
					sound: "Camel.mp3"
				},
				{
					title: "Polar bear",
					sound: "Polarbear.mp3"
				},
				{
					title: "Dress",
					sound: "Dress.mp3"
				},
				{
					title: "Bed",
					sound: "Bed.mp3"
				},
				{
					title: "Ball",
					sound: "Ball.mp3"
				},
				{
					title: "Shorts",
					sound: "Shorts.mp3"
				},
				{
					title: "Trousers",
					sound: "Trousers.mp3"
				},
				{
					title: "House",
					sound: "House.mp3"
				},
				{
					title: "Strawberries",
					sound: "Strawberries.mp3"
				},
				{
					title: "Thankyou",
					sound: "Thankyou.mp3"
				},
				{
					title: "Boots",
					sound: "Boots.mp3"
				},
				{
					title: "Pyjamas",
					sound: "Pyjamas.mp3"
				},
				{
					title: "Swingsuit",
					sound: "Swingsuit.mp3"
				},
				{
					title: "Morning",
					sound: "Morning.mp3"
				},
				{
					title: "Afternoon",
					sound: "Afternoon.mp3"
				},
				{
					title: "Evening",
					sound: "Evening.mp3"
				},
				{
					title: "Living room",
					sound: "livingroom.mp3"
				},
				{
					title: "Bedroom",
					sound: "bedroom.mp3"
				},
				{
					title: "Kitchen",
					sound: "kitchen.mp3"
				},
				{
					title: "Grandfather",
					sound: "grandfather.mp3"
				},
				{
					title: "Grandmother",
					sound: "grandmother.mp3"
				},
				{
					title: "Family",
					sound: "family.mp3"
				},
				{
					title: "Coat",
					sound: "coat.mp3"
				},
				{
					title: "Skirt",
					sound: "skirt.mp3"
				},
				{
					title: "Jacket",
					sound: "jacket.mp3"
				},
				{
					title: "Shoes",
					sound: "shoes.mp3"
				},
				{
					title: "Parrot",
					sound: "parot.mp3"
				},
					{
					title: "Snake",
					sound: "snake.mp3"
				},
					{
					title: "Cheetah",
					sound: "cheetah.mp3"
				},
					{
					title: "Mother",
					sound: "mother.mp3"
				},
					{
					title: "Father",
					sound: "father.mp3"
				},
					{
					title: "Cat",
					sound: "cat.mp3"
				},
					{
					title: "Dog",
					sound: "dog.mp3"
				},
					{
					title: "Mouse",
					sound: "mouse.mp3"
				}
			]
		}
	},
	methods: {
		play: function (name) {
			let audio = new Audio(require('@/assets/sounds/' + name));
			audio.play();
		}
	}
}
</script>

