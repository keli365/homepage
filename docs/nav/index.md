---
layoutClass: m-nav-layout
outline: [2, 3, 4]
---

<script setup>
import { NAV_DATA } from './data'
</script>
<style src="./index.scss"></style>

# 前端导航

<MNavLinks v-for="{title, items} in NAV_DATA" :title="title" :items="items"/>

<br />

export default defineConfig({
    ---
    socialLinks: [{ icon: 'github', link: 'https://github.com/maomao1996/vitepress-nav-template' }], //社交链接

    footer: {
      copyright: 'Copyright © Keli365 | maomao'
    },  //页脚，可按Vue支持格式修改
})
