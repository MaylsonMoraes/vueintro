<template>
    <form action="">
        <div>
        <inputText />
        </div>
        <div>
        <inputText />
        </div>
        <div>
        <Customsubmit /> 
        </div>
    </form>
</template>
<script>
import inputText from './Form/inputText'
import Customsubmit from './Form/submit'

export default {
    name:'Customform',
    components: {
        inputText,
        Customsubmit
    }
}
</script>
