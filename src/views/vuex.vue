<template>
    <div>
        vuex
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import axios from '../utils/axios';

export default defineComponent({
    setup() {
        axios.get('/user/XPoet').then(res => {
            console.log(res,'res')
        }).catch(err => {
            console.log(err,'err')
        })
    }
})
</script>

<style lang="stylus">

</style>
