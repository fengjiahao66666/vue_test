<template>
    <div class="demo">
        <h2>学生姓名：{{name}}</h2>
        <h2>学生年龄：{{age}}</h2>
    </div>
</template>
<script>
// export const school = Vue.extend({//分别暴露
//         data(){
//             return {
//                 schoolName:'尚硅谷',
//                 address:'北京昌平'
//             }
//         },
//         methods: {
//             showName(){
//                 alert(this.schoolName)
//             }
//         },
//     })

    // const school = Vue.extend({
    //     data(){
    //         return {
    //             schoolName:'尚硅谷',
    //             address:'北京昌平'
    //         }
    //     },
    //     methods: {
    //         showName(){
    //             alert(this.schoolName)
    //         }
    //     },
    // })
    // export{school}//统一暴露

    // const school = Vue.extend({
    //     data(){
    //         return {
    //             schoolName:'尚硅谷',
    //             address:'北京昌平'
    //         }
    //     },
    //     methods: {
    //         showName(){
    //             alert(this.schoolName)
    //         }
    //     },
    // })
    // export default school //默认暴露

    export default{
        name:'StudentName',
        data(){
            return {
                name:'张三',
                age:18
            }
        },
    }
    
</script>

<style>

</style>