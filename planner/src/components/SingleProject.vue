<template>
    <div class="project">
        <div class="actions">
<h3 @click="showDetails =! showDetails">{{project.title}}</h3>
<div class="icon">
<span class="material-icons-outlined">

</span>
</div>

        </div>
        <div class="details" v-if="showDetails">
<h5>{{project.details}}</h5>
        </div>
        

    </div>
</template>

<script>
export default{
props:['project'],
data(){
    return{
        showDetails: false
    }
}
}

</script>

<style lang="scss" scoped>
.project {
    margin: 20px auto;
    background-color: white;
    padding: 10px 20px;
    box-shadow: 1px 2px 3 px rbga(0,0,0,0.05);
    border-left: 4px solid #e90074;
}
h3 {
    cursor: pointer;
}
h5{
    
}
</style>
