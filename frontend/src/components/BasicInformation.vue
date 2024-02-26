<template>
    <div class="basic-info">
        <div class="part1">部分1</div>
        <div class="part2">部分2</div>
    </div>
</template>
  
<script>
export default {
    name: 'BasicInformation',
};
</script>
  
<style scoped>
.basic-info {
    display: grid;
    grid-template-rows: 1fr 4fr;
    height: 100%;
}

.part1,
.part2 {
    border: 2px solid purple;
    margin: 2px;
}
</style>