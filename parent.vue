<template>
    <div>
        <LamChild v-for="(gameItem,index) in gameItems"  :imgurl="gameItem.urlIcon" :name="gameItem.name" :des="gameItem.des" :score="gameItem.score" :key="index"></LamChild>
    </div>
    
</template>
<script setup>

    const gameItem1 = ref({
        urlIcon:'https://cdn.dribbble.com/users/3738618/screenshots/17359053/media/17d11f0609df07a3edf690279cf808c1.png?resize=1000x750&vertical=center',
        name:'Game 1',
        des:'This is game 1',
        score:100
    })

    const gameItem2 = ref({
        urlIcon:'https://cdn.dribbble.com/users/3738618/screenshots/17359053/media/17d11f0609df07a3edf690279cf808c1.png?resize=1000x750&vertical=center',
        name:'Game2',
        des:'This is game 2',
        score:200
    })

    const gameItems = ref([]);
    gameItems.value.push(gameItem1);
    gameItems.value.push(gameItem2);

</script>