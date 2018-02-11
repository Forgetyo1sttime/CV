<template>
    <div class="col-sm-4 col">
        <h2></h2> 

        <div class="card">
            <div class="card-body">
                <h2 class="card-title">{{skill.title}}</h2>
                <p class="card-text">{{skill.content}}</p>
                <img :src="skill.main_image" class="img-thumbnail"/>
            <br/>
            <img v-for="image in skill.images" :key="image" :src="image" class="img-thumbnail small-image"/>
            </div>
        </div>
    
    </div>
</template>

<script>
export default {
  name: "Skill",
  props: ["skill"]
};
</script>

<style scoped>
    .small-image {
        display:inline;
        margin: 2px;
        max-width:200px; 
        max-height:100px
    }

    img {
        max-height: 232px;
        margin-top: 10px;
    }
</style>
