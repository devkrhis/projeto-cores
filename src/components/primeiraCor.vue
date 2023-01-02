<template>
    <div id="primeiraCor">
        <h1> Essa cor é: {{ vermelho }}</h1>
        <button type="button" @click="changeColor"> Randon Color</button>
        <button type="button" :applyChange="{apllyColor refazer}"></button>
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
            apllyColor: 'True', // Aplicar mudança de cor e ver como ficou
            noApllyColor: 'False'
        }
    },
    methods: {
        changeColor(){

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