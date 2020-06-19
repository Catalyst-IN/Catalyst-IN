<template>
  <agile
    :rtl="false"
    :dots="true"
    :infinite="true"
    :autoplay="true"
    :autoplay-speed="5000"
    :pauseOnHover="true"
    :centerMode="true"
  >
    <div class="slide">
      <a href="https://github.com/Catalyst-IN/Awesome-10-20-Frontend" target="_blank"
        ><img src="../assets/e1020.png"
      /></a>
    </div>
    <div class="slide">
      <a
        href="https://github.com/Catalyst-IN"
        target="_blank"
        ><img src="../assets/event2.png"
      /></a>
    </div>
    <!--    <div class="slide">-->
    <!--      <a href="https://github.com/Catalyst-IN" target="_blank"-->
    <!--        ><img src="../assets/event4.png"-->
    <!--      /></a>-->
    <!--    </div>-->
    <template slot="prevButton"><i class="fas fa-chevron-left"></i></template>
    <template slot="nextButton"><i class="fas fa-chevron-right"></i></template>
  </agile>
</template>

<script>
import { VueAgile } from "vue-agile";
export default {
  components: {
    agile: VueAgile,
  },
};
</script>

<style lang="sass">
// VueAgile styles
.agile
	&__nav-button
		background: transparent
		border: none
		color: #fff
		cursor: pointer
		font-size: 24px
		height: 100%
		position: absolute
		top: 0
		transition-duration: .3s
		width: 80px

		&:hover
			background-color: rgba(#000, .5)
			opacity: 1

		&--prev
			left: 0

		&--next
			right: 0

	&__dots
		bottom: 10px
		left: 50%
		position: absolute
		transform: translateX(-50%)

	&__dot
		margin: 0 10px

		button
			background-color: transparent
			border: 1px solid #fff
			border-radius: 50%
			cursor: pointer
			display: block
			height: 10px
			font-size: 0
			line-height: 0
			margin: 0
			padding: 0
			transition-duration: .3s
			width: 10px

		&--current,
		&:hover
			button
				background-color: #fff

// Slides styles
.slide
	display: block
	height: 500px
	object-fit: cover
	width: 100%
.slide img
  width: 100%
  height: 100%
  overflow: hidden
</style>
