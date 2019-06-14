<template>
<div>
<div class="right">
    <div>
<b-button v-b-toggle.collapse-1 variant="primary">Add a Movie</b-button>
  <b-collapse id="collapse-1" class="mt-2">
      <p class="card-text"/>
      <form @submit.prevent="addmovie">
  <input type="text" placeholder="Enter movie Name"  required v-model="title" autofocus="yes" >
  <input type="url" placeholder="Enter the poster Url" v-model="url" autofocus="yes">
  <textarea required placeholder="Enter breif summary about the Movie" v-model="summary" cols="22" rows="3" autofocus="yes" />
  <div>
      <b-button type="submit" variant="primary">Submit</b-button>
      <b-button type="reset" variant="danger">Reset</b-button>
  </div>
      </form>

</b-collapse>
</div>
</div>
<div class="gallery">
  <a target="_blank" >
    <b-img :src="url" :alt="title" width="600" height="400"  @click="$bvToast.show('example-toast')"/>  </a>
    <b-toast id="example-toast" title="Summary" static no-auto-hide>
      {{summary}}
    </b-toast>
  <div class="desc">{{title}}</div>

</div>

 
</div>
</template>

<script>
  export default {

  data (){
    return{
      title:'',
      url:'',
      summary:''
    }
  }
  } 
</script>

<style>
.right {
  position: absolute;
  right: 0px;
  width: 300px;
  padding: 10px;
}

div.gallery {
  margin: 5px;
 
  float: left;
  width: 180px;
}

div.gallery:hover {
  border: 1px solid #777;
}

div.gallery img {
  width: 100%;
  height: auto;
}

div.desc {
  padding:10px;
  text-align: center;
}
</style>
