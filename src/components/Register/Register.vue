<template>
    <div class="container text-center mt-5">
       <div class="card">
           <div class="form-group">
            <label for="exampleInputEmail1">Email address</label>
            <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="Enter email" v-model="user.email">
            
            </div>
            <div class="form-group">
                <label for="exampleInputPassword1">Password</label>
                <input type="password" class="form-control" id="exampleInputPassword1" placeholder="Password" v-model="user.password">
            </div>
            
            <button @click="btnalert" class="btn btn-primary">Submit</button> <br>
                {{ user.email}} <br>
                {{ user.password }}
       </div>  
    </div>
</template>

<script>
export default {
    data() {
        return {
            user : { 
                email: "",
                password: ""
            }
        }
    },
    methods: {
        btnalert() {
            alert(this.user.email)
        }
    }
   
    
}
</script>

<style scoped>
   
</style>