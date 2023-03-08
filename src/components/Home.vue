<template>
<div>
    <h1>For loop in Vue.js</h1>
    <table border=1px>
        <tr>
            <td>Id</td>
            <td>Name</td>
            <td>Email</td>
        </tr>
        <tr v-for="user in users" :key="user.id">
            <td>{{user.id}}</td>
            <td>{{user.name}}</td>
            <td>{{user.email}}</td>
        </tr>
    </table>
</div>
</template>

<script>
export default {
    name:"appHome",
    props: {
        data:String,
        msg: String
    }, data(){
        return {
            users:[
                {  id:1,name:'deepak',email:'deep@gmail.com'
                },
                {  id:2,name:'taj',email:'taj@gmail.com'
                },
                {  id:3,name:'kavya',email:'kavya@gmail.com'
                },
                {  id:4,name:'kk',email:'kk@gmail.com'
                }
            ]
        }
    }

}
</script>