<template>
<div>
    <button v-on:click="display">Toggle Show</button>
    <button v-if="show" v-on:click="helloAlert">hello Alert is Active</button>
    <button v-else>hello</button>
    <table border="2px">
    <tr>
        <td>ID</td>
        <td>User Name</td>
        <td>Email Address</td>
        </tr>
        <tr v-for="user in users" :key="user.id">
            <td>{{user.id}}</td>
            <td>{{user.name}}</td>
            <td>{{user.mail}}</td>
    </tr>
    </table>
    <h1>Hello From Home component</h1>
    <p>{{CopyrightNotice}}</p>
</div>
</template>

<script>


    export default{
        name:"HomeComponent",
        props:{
            CopyrightNotice:String,
        },
        
            helloAlert()
            {
                alert("Hello, There How can I help you??");
            },
            data()
            {
        
                return {show:false}
            },


            methods:
            {
                displayUsersInfo()
                {
                    if(this.show)
                    {
                        return {users:[{id:1,name:"Vishal Ahirwar",mail:"thisismail@vmail.com"},
                                        {id:2,name:"Cishal Ahirwar",mail:"thisiCmail@vmail.com"},
                                        {id:3,name:"Hishal Ahirwar",mail:"thiHsismail@vmail.com"}
                                        ]
                                }
                    }else
                    {
                        return{users:[]}
                    }
                }
,
                display()
                {
                    this.show=!this.show
                },
            }
    }
</script>
