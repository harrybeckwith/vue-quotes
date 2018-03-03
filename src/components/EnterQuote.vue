<template>
    <div>
        <app-prog-bar :count='count'>
            {{count }}
        </app-prog-bar>
        <hr>
        <input type='text' />
        <button @click='increaseCount'>Add quote</button>

    </div>
</template>
<script>
    import ProgBar from './progBar.vue';
    export default {
        components: {
            appProgBar: ProgBar
        }, methods: {
            increaseCount() {
                this.count++;
            }
        },
        data: function () {
            return {
                count: 0
            }
        }
    }
</script>