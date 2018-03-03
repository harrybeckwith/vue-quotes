<template>
    <div class='progBar' :style="{ backgroundImage: 'url(' + count + ')' }">

        progression: {{count}}
    </div>
</template>
<script>
    export default {
        props: ['count']


    }
</script>