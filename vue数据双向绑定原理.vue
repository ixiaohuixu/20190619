<template>
    <div>
        <input type="text" v-model="word">
        <p>{{word}}</p>
        <button v-on:click="sayHi"></button>
    </div>
</template>

<script>
    export default {
        var vm = new MVVM({
            el:'#mvvm-app',
            data:{
                word:'hello world'
            },
            methods:{
                sayHi:function(){
                    this.word = 'Hi,everybody'
                }
            }
        })
    }
</script>

<style lang="stylus" rel="stylesheet/stylus">

</style>
