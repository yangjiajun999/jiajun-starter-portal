<template>
    <a-layout id="components-layout-demo-side" style="min-height: 100vh">
        <a-layout-sider v-model="collapsed" collapsible>
            <div class="logo">后台管理系统</div>
            <a-menu theme="dark" :defaultSelectedKeys="['1']" mode="inline">
                <a-menu-item key="1">
                    <a-icon type="pie-chart" />
                    <span>Option 1</span>
                </a-menu-item>
                <a-menu-item key="2">
                    <a-icon type="desktop" />
                    <span>Option 2</span>
                </a-menu-item>
                <a-sub-menu
                    key="sub1"
                >
                    <span slot="title"><a-icon type="user" /><span>User</span></span>
                    <a-menu-item key="3">Tom</a-menu-item>
                    <a-menu-item key="4">Bill</a-menu-item>
                    <a-menu-item key="5">Alex</a-menu-item>
                </a-sub-menu>
                <a-sub-menu
                    key="sub2"
                >
                    <span slot="title"><a-icon type="team" /><span>Team</span></span>
                    <a-menu-item key="6">Team 1</a-menu-item>
                    <a-menu-item key="8">Team 2</a-menu-item>
                </a-sub-menu>
                <a-menu-item key="9">
                    <a-icon type="file" />
                    <span>File</span>
                </a-menu-item>
            </a-menu>
        </a-layout-sider>
        <a-layout>
            <a-layout-header style="background: #fff; padding: 0">
                <a-menu mode="horizontal">
                    <a-sub-menu>
                        <span slot="title" class="submenu-title-wrapper"><a-icon type="usergroup-add" />人员管理</span>
                        <a-menu-item key="setting:1">用户管理</a-menu-item>
                        <a-menu-item key="setting:2">角色管理</a-menu-item>
                    </a-sub-menu>
                    <a-sub-menu>
                        <span slot="title" class="submenu-title-wrapper"><a-icon type="setting" />系统管理</span>
                        <a-menu-item key="setting:3">Option 1</a-menu-item>
                        <a-menu-item key="setting:4">Option 2</a-menu-item>
                    </a-sub-menu>
                </a-menu>
            </a-layout-header>
            <a-layout-content style="margin: 0 16px">
                <nuxt />
            </a-layout-content>
            <a-layout-footer style="text-align: center">
                Admin Template ©2019 Created by JiaJun Yang
            </a-layout-footer>
        </a-layout>
    </a-layout>
</template>
<script>
export default {
    data() {
        return {
            collapsed: false,
        };
    },
};
</script>

<style lang="stylus">
    .ant-layout-header
        height auto
    #components-layout-demo-side .logo
        height 33px
        line-height 33px
        margin 5px
        text-align center
        color #fff
        overflow hidden
        font-size 15px
        background rgba(255,255,255,0.2)
</style>
