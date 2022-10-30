<demo>
基础用法
</demo>
<template>
    <div>示例1</div>
    <Tabs v-model:selected="x">
        <Tab title="用户管理">用户管理</Tab>
        <Tab title="配置管理">配置管理</Tab>
        <Tab title="角色管理">角色管理</Tab>
    </Tabs>
</template>
<script lang="ts">
import Tabs from '../../lib/Tabs.vue'
import Tab from '../../lib/Tab.vue'
import {ref} from 'vue'
export default {
    components:{Tabs,Tab},
    setup() {
        const x = ref('用户管理')
        return {x}
    }
}
</script>