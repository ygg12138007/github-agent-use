<script setup>
// Vue简介页面组件
</script>

<template>
    <div class="vue-intro-container">
        <header class="vue-header">
            <h1>Vue.js 简介</h1>
        </header>

        <main class="vue-content">
            <section class="what-is-vue">
                <h2>什么是 Vue.js？</h2>
                <p>Vue.js 是一个渐进式 JavaScript 框架，用于构建用户界面。它是一个专注于视图层的框架，易于上手，同时也能够与其他库或现有项目集成。</p>
                <p>Vue 由 Evan You 创建，其核心库只关注视图层，不仅易于上手，还便于与第三方库或既有项目整合。</p>
            </section>

            <section class="vue-features">
                <h2>Vue.js 的主要特点</h2>
                <ul>
                    <li><strong>响应式数据绑定</strong>：当数据发生变化时，视图会自动更新</li>
                    <li><strong>组件化</strong>：允许将界面拆分为可复用的组件</li>
                    <li><strong>虚拟 DOM</strong>：提高页面渲染性能</li>
                    <li><strong>指令系统</strong>：提供了丰富的内置指令，如 v-model、v-for、v-if 等</li>
                    <li><strong>轻量级</strong>：体积小，加载速度快</li>
                    <li><strong>易于学习</strong>：API 设计简洁明了，学习曲线平缓</li>
                </ul>
            </section>

            <section class="vue-advantages">
                <h2>Vue.js 的优势</h2>
                <div class="advantage-cards">
                    <div class="advantage-card">
                        <h3>渐进式框架</h3>
                        <p>可以根据需求逐步采用，从简单的表单处理到复杂的单页应用都能胜任</p>
                    </div>
                    <div class="advantage-card">
                        <h3>性能优异</h3>
                        <p>高效的虚拟 DOM 实现和响应式系统，确保了优秀的性能表现</p>
                    </div>
                    <div class="advantage-card">
                        <h3>生态系统完善</h3>
                        <p>拥有丰富的官方和社区插件，可以满足各种开发需求</p>
                    </div>
                    <div class="advantage-card">
                        <h3>文档详尽</h3>
                        <p>提供了全面且易于理解的中文和英文文档</p>
                    </div>
                </div>
            </section>

            <section class="vue-use-cases">
                <h2>Vue.js 的应用场景</h2>
                <p>Vue.js 适用于各种规模的项目：</p>
                <ul>
                    <li>单页应用（SPA）</li>
                    <li>复杂的企业级前端应用</li>
                    <li>移动应用开发（通过 Weex 或 Quasar 等框架）</li>
                    <li>服务端渲染（SSR）应用</li>
                    <li>作为现有项目的一部分进行增强</li>
                </ul>
            </section>
        </main>

        <footer class="vue-footer">
            <p>了解更多关于 Vue.js 的信息，请访问 <a href="https://cn.vuejs.org/" target="_blank">官方网站</a></p>
        </footer>
    </div>
</template>

<style lang="scss" scoped>
// 颜色变量定义
$primary-color: #4fc08d;
$text-color: #333;
$light-text: #666;
$bg-color: #f9f9f9;
$card-bg: white;
$border-color: #ddd;

// 尺寸变量
$border-radius: 8px;
$spacing: 20px;
$section-margin: 40px;

.vue-intro-container {
    max-width: 1200px;
    margin: 0 auto;
    padding: $spacing;
    color: $text-color;

    .vue-header {
        text-align: center;
        margin-bottom: $section-margin;

        h1 {
            color: $primary-color;
            font-size: 2.5em;
            margin: 0;
        }
    }

    .vue-content {
        line-height: 1.6;

        section {
            margin-bottom: $section-margin;
            padding: $spacing;
            background-color: $bg-color;
            border-radius: $border-radius;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);

            h2 {
                color: $text-color;
                border-bottom: 2px solid $primary-color;
                padding-bottom: 10px;
                margin-bottom: 20px;
            }

            p {
                margin-bottom: 15px;
            }

            ul {
                margin-left: 20px;
                margin-bottom: 20px;

                li {
                    margin-bottom: 8px;
                }
            }
        }

        // 优势卡片样式
        .advantage-cards {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: $spacing;
            margin-top: $spacing;

            .advantage-card {
                background-color: $card-bg;
                padding: $spacing;
                border-radius: $border-radius;
                box-shadow: 0 2px 4px rgba(0, 0, 0, 0.05);
                transition: transform 0.3s ease;

                &:hover {
                    transform: translateY(-5px);
                }

                h3 {
                    color: $primary-color;
                    margin-top: 0;
                    margin-bottom: 10px;
                }
            }
        }
    }

    .vue-footer {
        text-align: center;
        margin-top: 60px;
        padding-top: $spacing;
        border-top: 1px solid $border-color;
        color: $light-text;

        a {
            color: $primary-color;
            text-decoration: none;

            &:hover {
                text-decoration: underline;
            }
        }
    }
}
</style>