<!--  -->
<template>
    <div class="Time" >
        <h3> {{time | formatData}} </h3>
    </div>
</template>

<script>

// 导入的其他文件 例如：import moduleName from 'modulePath';

    export default {
        name: 'HelloTime',
        data() {
            return {
                time: new Date ()
            }
        },

        filters: {
            formatData : function (value){
                var date = new Date(value);
                var year = date.getFullYear();
                var month = date.getMonth() + 1;
                var day = date.getDate();
                var hours = date.getHours();
                var minutes = date.getMinutes();
                var seconds = date.getSeconds();
                var s = year + '-' + month + '-' + day + ' ' +  hours + ':' + minutes + ':' + seconds;
                return s;
            }

        },
        //挂载完成 访问DOM元素
        mounted() {
            var _this = this;
            this.timer = setInterval(() => {
                _this.time = new Date ();
            }, 1000);

        },

        //组件销毁之前调用
        beforeDestroy() {
            if (this.timer) {
                clearInterval(this.timer);
            }
        }
    }
</script>

<style  scoped>
h3 {
  margin: 40px 0 0;
}
#Time {
  color: #eb0000;
}
</style>