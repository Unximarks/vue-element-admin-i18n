<template>
  <div class="block">
    <el-timeline>
      <el-timeline-item v-for="(item,index) of timeline" :key="index" :timestamp="item.timestamp" placement="top">
        <el-card>
          <h4>{{ item.title }}</h4>
          <p>{{ item.content }}</p>
        </el-card>
      </el-timeline-item>
    </el-timeline>
  </div>
</template>

<script>
export default {
  data() {
    return {
      timeline: [
        {
          timestamp: '2020/12/16',
          title: 'js 实现纯前端将数据导出excel两种方式',
          content: '内容太复杂，略~'
        },
        {
          timestamp: '2020/10/21',
          title: 'JavaScript知识点-周1.md',
          content: 'javascript是基于对象和事件驱动的解释性脚本语言;'
        },
        {
          timestamp: ' 2020/09/26',
          title: 'HTML+CSS知识点-周3.md',
          content: '定位元素的层级设置： 设置了定位的元素可以通过z-index属性调整层级关系，默认值都是0，数字越大层级越高，数字相同，层级跟标签的顺序有关，标签越靠后层级越高'
        },
        {
          timestamp: '2020/08/14',
          title: 'Vue学习day3.md',
          content: '一个vue实例生命的周期，也就是vue实例从开始到结束的过程，从创建到销毁的过程'
        }
      ]
    }
  }
}
</script>
