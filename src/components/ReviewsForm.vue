<template>
    <Card>
        <form>
            <h2>
                How would you rate your service with us?
                <!--Rating component-->
                <div class="input-group">
                    <input type="text" placeholder="Write a review" v-model="text">
                    <button type="submit" class="btn btn-primary" :disabled="btnDisabled"></button>
                </div>
                <div class="message">Text must be at least 10 characters</div>
            </h2>
        </form>
    </Card>

</template>

<script setup>
import { ref } from 'vue'
import Card from './shared/Card.vue'

const text = ref('');
const btnDisabled = ref(false);
const message = ref('')
</script>

<style >

</style>