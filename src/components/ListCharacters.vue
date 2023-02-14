<template lang="">
    <section>
        <div class="characters">
            <div class="characters__item"></div>
            <h2>Characters</h2>
        </div> 
    </section>
</template>
<script>
import { onMounted } from 'vue';
import { useStore } from 'vuex'
export default {
    setup(){
        const store = useStore()
        onMounted(() =>{
        store.dispatch('getCharacter')
    })
    }
}
</script>
<style lang="">
    
</style>