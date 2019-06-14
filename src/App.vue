<template>
 <div id='app'>
<Navigation />
<Movie />
<Form/>

  </div>
</template>

<script>
import Navigation from './components/Navigation.vue'
import Movie from './components/Movie.vue'
import Form from './components/Form.vue'

export default
{
	components :{
Navigation,
Movie,
 Form
	}
}
</script>

<style >
body{
background: green;
}

</style>
