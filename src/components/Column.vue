<script>
export default {
    data: () => {
        return {
            inputName: "",
            inputPercent: 0,
            savedData:{
                inputName: '',
                inputPercent: 0,
            }
        }
    },
    computed:{
    },
    methods:{
        saveData(){
            this.savedData.inputName = this.inputName,
            this.savedData.inputPercent = this.inputPercent
        }
    },
}
</script>

<template>
<div class="block">
    <input type="text" placeholder="Название" v-model="inputName" >
    <input type="number" placeholder="Процент" v-model="inputPercent" >
    <button @click="saveData">Сохранить</button>
    <div class="inner--block">
        <div class="box">
            <div :style="{
                height: savedData.inputPercent + '%',
                backgroundColor: 'blue',
            }">
            </div>
        </div>
        <p>{{savedData.inputName}}</p>
    </div>
    
</div>
</template>

<style scoped>
.block{
    width: 300px;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 20px;
}
.inner--block{
    text-align: center;
}
.box{
    width: 200px;
    height: 300px;
    border: 1px solid black;
}

</style>