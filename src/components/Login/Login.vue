<template>
    <div class="container text-center mt-5">
        <hr>
        name <br>
        <input type="text" placeholder="name" name="" id="" v-model="user.name"> <hr><br>
        username <br>
        <input type="text" placeholder="username" name="" id="" v-model="user.username">      
        <hr><br>
        <button class="btn btn-primary" @click="btnalert">
            Submit
        </button>
        <br><hr>
        {{ user.name }}
        {{ user.username }}
    </div>
</template>

<script>
export default {
    data() {
        return {
            user : { 
                name: "sait",
                username: "enes"
            }
        }
    },
    methods: {
        btnalert() {
            alert( this.user.name )
        }
    },
    computed:{

    },
    created() {
        
    },
    
}
</script>

<style scoped>
    .header { 
        margin-top: 150px;
    }
</style>