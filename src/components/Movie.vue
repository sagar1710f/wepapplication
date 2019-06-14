<template>
<div>

<div class="media-body">
<div class="gallery">
 
    <img src="https://bit.ly/2IcnSwz" alt="Harry Potter and the Order of the Phoenix" width="600" height="400"  @click="$bvToast.show('movie1')" />
   <div class="desc"> Harry Potter and the Order of the Phoenix </div>
      <b-toast id="movie1" title="Summary" static no-auto-hide>
Harry Potter and Dumbledores warning about the return of Lord Voldemort is not heeded by the wizard authorities who, in turn, look to undermine Dumbledores authority at Hogwarts and discredit Harry'
    </b-toast>
  </div>
<div class="gallery">
      <img src="https://bit.ly/2tC1Lcg" alt="The Lord of the Rings: The Fellowship of the Ring" width="600" height="400" @click="$bvToast.show('movie2')" /> 
   <div class="desc">The Lord of the Rings:The Fellowship of the Ring</div>
<b-toast id="movie2" title="Summary" static no-auto-hide>
  A young hobbit, Frodo, who has found the One Ring that belongs to the Dark Lord Sauron, begins his journey with eight companions to Mount Doom, the only place where it can bedestroyed. 
   </b-toast>

</div>

<div class="gallery">

    <img src="https://bit.ly/2Pzczlb" alt="Avengers: Endgame" width="600" height="400" @click="$bvToast.show('movie13')" >
  <div class="desc">Avengers: Endgame  </div>
<b-toast id="movie23" title="Summary" static no-auto-hide>
Adrift in space with no food or water, Tony Stark sends a message to Pepper Potts as his oxygen supply starts to dwindle. Meanwhile, the remaining Avengers -- Thor, Black Widow, Captain America and Bruce Banner -- must figure out a way to bring back their vanquished allies for an epic showdown with Thanos -- the evil demigod who decimated the planet and the universe.
 </b-toast>

</div>
</div >
</div>
</template>

<script>


export default{


}

</script>

<style>
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
