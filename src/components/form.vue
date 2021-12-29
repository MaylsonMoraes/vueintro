<template>
    <form action="">
        <div>
        <inputText />
        </div>
        <div>
        <inputText />
        </div>
        <div>
        <submit />
        </div>
    </form>
</template>
<script>
import inputText from './Form/inputText.vue'
import submit from './Form/submit.vue'

export default {
    name:'form',
    components: {
        inputText ,
        submit
    }
}
</script>
