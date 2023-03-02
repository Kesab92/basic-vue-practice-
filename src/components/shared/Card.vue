<template>
    <div class="card" :class="{'reverse':reverse}">
        <slot></slot>

    </div>
</template>

<script>

export default {
    name: 'Card',
    props:{
        type: Boolean,
        default:false,
    },
}

</script>

<style >
    .card{
        background: #fff;
        color: #212121;

    }
    .card.reverse{
        background:#212121;
        color:#fff;
    }
</style>