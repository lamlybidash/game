<template>
    
    <div class="flex">
        <div>
            <UiImg class="w-10 h-10" :src="props.imgurl"></UiImg>
        </div>

        <div>
            {{ props.name }}
        </div>
        
        <div>
            {{ props.des }}
        </div>

        <div>
            {{ props.score }}
        </div>

    </div>

</template>

<script setup>
    const props = defineProps(['imgurl', 'name','des','score'])   
</script>