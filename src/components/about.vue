<template>
    <div class="about">
        <h1>{{ msg }}</h1>
    </div>
</template>

<script>
    export default {
        name: 'AboutComponent',
        props: {
            msg: String
        }
    }
</script>