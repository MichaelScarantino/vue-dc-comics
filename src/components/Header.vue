<template>
  <header>
    <div class="container">
        ciao sono un header
    </div>
  </header>
</template>

<script>
export default {
  name: "Header"
};
</script>

<style scoped lang="scss">
    @import '../style/variables.scss';

    header{
        width: 100%;
        height: 80px;

        // TEST
        background-color: cadetblue;
    }

</style>
