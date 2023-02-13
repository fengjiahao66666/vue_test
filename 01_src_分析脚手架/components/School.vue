<template>
    <div class="demo">
        <h2>学校名称：{{schoolName}}</h2>
        <h2>学校地址：{{address}}</h2>
        <button @click="showName">点我提示学校名</button>
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
        name:'SchoolName',
        data(){
            return {
                schoolName:'尚硅谷',
                address:'北京昌平'
            }
        },
        methods: {
            showName(){
                alert(this.schoolName)
            }
        },
    }
    
</script>

<style>
.demo{
    background-color: blue;
}
</style>