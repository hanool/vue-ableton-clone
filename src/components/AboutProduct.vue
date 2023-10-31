<template>
	<div class="about-product">
		<div class="first">
			div1
		</div>
		<div class="second">
		</div>
		<div class="third">
			div3
		</div>
	</div>
</template>

<style scoped>
.about-product {
	position: relative;
}

.first {
  position: absolute;
  left: 666.66667px;
  width: 933.33333px;
  height: 933.33333px;
  background-color: yellow;
}

.second {
  margin-left: 133.3333px;
  width: 666.66667;
  height: 666.66667;
  background-color: red;
  display: inline-block;
  vertical-align: middle;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: 50% 50%;
  background-image: url('@/assets/photo-1.jpg');
}
</style>
