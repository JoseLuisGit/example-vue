<template>
  <h1>{{ customTitle }}</h1>
  <p>  {{ counter }} <sup>2</sup> = {{ toSquareCounter }} </p>
  <button @click="increment">+1</button>
  <button @click="decrement">-1</button>
</template>

<script>
export default {

    props:{
        title: String,
        start: {
            type: Number,
            required: false,
            default: 10
        }
    },
    //name:'Hello',
    data(){
        return {
            counter: this.start,
        }
    },
    methods:{
        increment(){
            this.counter++;
        },
        decrement(){
            this.counter--;
        }
    },
    computed:{
        toSquareCounter(){
            return this.counter * this.counter;
        },

        customTitle(){
            return this.title || 'Counter';
        }
    }
}
</script>

<style>

    button{
        border-radius: 5px;
        background-color: #648687;
        border: 1px solid white;
        color: white;
        cursor:pointer;
        margin: 0 5px;
        padding: 5px 15px;
        transition: 0.3s case-in-out;
    }

    button:hover{
        background-color: #5aa67b;
        transition: 0.3s case-in-out
    }

</style>