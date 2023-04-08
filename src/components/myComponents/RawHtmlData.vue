<script>
export default {
    data(){
        return{
            title: "This is My Title for Monday",
            person:{
                id:1,
                name:'Bill',
                img:"https://www.tvmovie.de/assets/2015/07/13/52010-25346516.jpg",
            },
            msg:"Bill uno de los integrantes de los cazafantasmas",
        }
    },
};
</script>

<template>
    <div>
        <h1>Holaa</h1>
        <h3>{{ title }}</h3>
        <div :id="person.id">
            <h4>{{ person.name }}</h4>
            <img :src="person.img" :alt="person.name"/>
        </div>
        <h5 v-html="msg"></h5>
    </div>
</template>

<style lang="css" scoped>
h3{
    color:pink;
}

h4{
    color:darkviolet
}

</style>