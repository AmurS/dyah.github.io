<template>
    <div class="site-footer">
        MIT Licensed | Copyright © 2023 <a class="vitepress" target="_blank" href="//dyah.rkgk.my.id/">{{ webTitle }}</a><br />
        Powered by <a class="vitepress" target="_blank" href="//vitepress.vuejs.org/">VitePress</a>
        | Theme by <a class="vitepress" target="_blank" href="//github.com/airene/vitepress-blog-pure">blog-pure</a>
        | <a class="vitepress" target="_blank" href="//up.korone.my.id">Server Status</a>
    </div>
</template>
<script lang="ts" setup>
import { useData } from 'vitepress'

const { site, theme } = useData()
const website = theme.value.website
const webTitle = site.value.title
</script>

<style>
.site-footer {
    color: #888;
    text-align: center;
    font-size: 0.75rem;
    width: 100%;
    padding: 15px 0;
    overflow: auto;
}
.vitepress {
    color: var(--vp-c-text-1);
    font-weight: 700;
}
</style>
