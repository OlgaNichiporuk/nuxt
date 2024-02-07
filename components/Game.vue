<script setup lang="ts">
type IArray = {
    number: String;
    question: String;
    answer_1: String;
    answer_2: String,
    answer_3: String,
    answer_4: String,
}
defineProps({
    question: String,
    number: String,
    answer_1: String,
    answer_2: String,
    answer_3: String,
    answer_4: String,
}
)
</script>

<template>
    <div class="container">
        <div class="number">{{ number }}</div>
        <div class="question">{{ question }}</div>
        <div class="answer">{{ answer_1 }}</div>
        <div class="answer">{{ answer_2 }}</div>
        <div class="answer">{{ answer_3 }}</div>
        <div class="answer">{{ answer_4 }}</div>

        <div class="button">Далее</div>
    </div>
</template>

    
<style lang="css">
.container {
    gap: 16px;
    display: flex;
    flex-direction: column;
    align-items: center;
    background-color: white;
    width: 800px;
    height: 360px;
    border-radius: 20px;
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    padding-bottom: 20px;
}

.number {
    font-size: 35px;
    text-align: center;
    letter-spacing: 0.2mm;
}

.question {
    font-size: 35px;
    text-align: center;
    letter-spacing: 0.2mm;
}

.answer {
    text-align: center;
    width: 200px;
    height: 50px;
    border-radius: 10px;
    border: 1.5px solid #535051;
    cursor: pointer;
    letter-spacing: 0.2mm;

}

.button {
    width: 100px;
    font-size: 25px;
    background-color: blueviolet;
    border-radius: 10px;
    text-align: center;
    color: white;
    cursor: pointer;
    letter-spacing: 0.4mm;

}
</style>