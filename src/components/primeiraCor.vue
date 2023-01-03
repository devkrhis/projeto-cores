<template>
    <div id="primeiraCor">
        <h1> Essa cor é: {{ vermelho }}</h1>
        <button type="button" @click="changeColor"> Randon Color</button>
        <hr>
        <h3> Aqui vai ser declarado o botão a onde se clica e volta para a cor neutra</h3>
        <corNeutra/>
    </div>
    
</template>

<script>
import corNeutra from './corNeutra.vue'

export default {
    components: {
        corNeutra
    },
    data(){
        return {
            vermelho: 'Red',
        }
    },
    methods: {
        changeColor(){
            this.vermelho = 'Blue'

        }
    }
}
</script>

<style scoped>
    #primeiraCor h1 {
        padding: 20px;
        margin: 1px solid black;
        background-color: red;
    }
</style>