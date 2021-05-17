<template>
  <fm-making-form ref="makingForm" upload preview generate-code generate-json clearable>
    <!-- 自定义操作区域插槽 -->
    <template slot="action">
      <span class="test-click" @click="testClick">点我操作</span>
    </template>
  </fm-making-form>
</template>

<script>
export default {
  mounted () {
  },
  methods:{
    testClick(){
      // getJSON	获取设计器配置的JSON数据	-
      // getHtml	获取设计器生成的可以直接使用的HTML代码	-
      // setJSON	设置设计器的配置信息	(value) 通过getJSON方法获取的JSON数据
      // clear	清空设计器
      console.log(this.$refs.makingForm.getJSON());
      
    }
  }
}
</script>
