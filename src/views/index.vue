<!-- <style scoped lang="less">
    .index{
        width: 100%;
        position: absolute;
        top: 0;
        bottom: 0;
        left: 0;
        text-align: center;
        h1{
            height: 150px;
            img{
                height: 100%;
            }
        }
        h2{
            color: #666;
            margin-bottom: 200px;
            p{
                margin: 0 0 50px;
            }
        }
        .ivu-row-flex{
            height: 100%;
        }
    }
</style> -->


<!-- <template>
    <div class="index">
        <Row type="flex" justify="center" align="middle">
            <Col span="24">
                <h1>
                    <img src="../images/logo.png">
                </h1>
                <h2>
                    <p>Welcome to your iView app!</p>
                    <Button type="ghost" @click="handleStart">Start iView</Button>
                </h2>
            </Col>
        </Row>
    </div>
</template>


<script>
    export default {
        methods: {
            handleStart () {
                this.$Modal.info({
                    title: 'Bravo',
                    content: 'Now, enjoy the convenience of iView.'
                });
            }
        }
    }
</script>
 -->







<!-- <template>
    <div> -->
        <!-- 导航栏 -->
       <!--  <Menu mode="horizontal" :theme="theme" active-name="1">
            <MenuItem name="1">
                <Icon type="ios-paper"></Icon>
                内容管理
            </MenuItem>

            <MenuItem name="2">
                <Icon type="ios-people"></Icon>
                用户管理
            </MenuItem>

            <Submenu name="3">
                <template slot="title">
                    <Icon type="stats-bars"></Icon>
                    统计分析
                </template>
                <MenuGroup title="使用">
                    <MenuItem name="3-1">新增和启动</MenuItem>
                    <MenuItem name="3-2">活跃分析</MenuItem>
                    <MenuItem name="3-3">时段分析</MenuItem>
                </MenuGroup>
                <MenuGroup title="留存">
                    <MenuItem name="3-4">用户留存</MenuItem>
                    <MenuItem name="3-5">流失用户</MenuItem>
                </MenuGroup>
            </Submenu>

            <MenuItem name="4">
                <Icon type="settings"></Icon>
                综合设置
            </MenuItem>

            <MenuItem name="5">
                <Icon type="ios-personadd"></Icon>
                个人中心
            </MenuItem>
        </Menu>
        <br> -->

        <!-- Grid栅格 -->
        <!-- <Row>
            <Col span="12">col-12</Col>
            <Col span="12">col-12</Col>
        </Row>
        <br>
        <Row>
            <Col span="8">col-8</Col>
            <Col span="8">col-8</Col>
            <Col span="8">col-8</Col>
        </Row>
        <br>
        <Row>
            <Col span="6">col-6</Col>
            <Col span="6">col-6</Col>
            <Col span="6">col-6</Col>
            <Col span="6">col-6</Col>
        </Row> -->





<!-- 
    </div>



</template>
<script>
    export default {
        data () {
            return {
                theme: 'dark'
            }
        } 
    }
</script> -->


<style scoped>
    .layout{
        border: 1px solid #d7dde4;
        background: #f5f7f9;
        position: relative;
        border-radius: 4px;
        overflow: hidden;
    }
    .layout-logo{
        width: 100px;
        height: 30px;
        background: #5b6270;
        border-radius: 3px;
        float: left;
        position: relative;
        top: 15px;
        left: 20px;
        text-align:center; 
        line-height: 30px;
        color: white;
    }
    .layout-nav{
        width: 500px;
        margin: 0 auto;
        margin-right: 20px;
    }
</style>

<template>
    <div class="layout">
        <Layout>

            
            <Header>
                <Menu mode="horizontal" theme="dark" active-name="1">
                    <div class="layout-logo">
                    Webank
                    </div>
                    <div class="layout-nav">
                        <MenuItem name="1">
                            <Icon type="ios-navigate"></Icon>
                            <span>工作区</span>
                        </MenuItem>
                        <MenuItem name="2">
                            <Icon type="ios-keypad"></Icon>
                            待办项
                        </MenuItem>
                        <MenuItem name="3">
                            <Icon type="ios-email"></Icon>
                            站内信
                        </MenuItem>
                        <MenuItem name="4">
                            <Icon type="ios-person"></Icon>
                            个人中心
                        </MenuItem>
                    </div>
                </Menu>
            </Header>

           
            <Layout>
                 <Sider hide-trigger collapsible:collapsed-width="78">
                    <Menu active-name="1-1" theme="dark" width=" auto " :open-names="['1']">
                        <Submenu name="1">
                            <template slot="title">
                                <Icon type="ios-navigate"></Icon>
                                工作平台
                            </template>
                            <MenuItem name="1-1">我的待办</MenuItem>
                            <MenuItem name="1-2">我的已办</MenuItem>
                            <MenuItem name="1-3">我的创建</MenuItem>
                        </Submenu>
                        <Submenu name="2">
                            <template slot="title">
                                <Icon type="ios-keypad"></Icon>
                                我的项目
                            </template>
                            <MenuItem name="2-1">项目管理工具</MenuItem>
                            <MenuItem name="2-2">PAMO RD</MenuItem>
                        </Submenu>
                        <Submenu name="3">
                            <template slot="title">
                                <Icon type="ios-analytics"></Icon>
                                创建项目
                            </template>
                            <MenuItem name="3-1">开发管理工具</MenuItem>
                            <MenuItem name="3-2">DEV test</MenuItem>
                        </Submenu>
                         <Submenu name="4">
                            <template slot="title">
                                <Icon type="ios-color-wand"></Icon>
                                T魔方
                            </template>
                            <MenuItem name="3-1">我的魔方秀</MenuItem>
                        </Submenu>
                    </Menu>
                </Sider>

               
                <Layout :style="{marginLeft: '0px'}">
                   
                    <Content :style="{padding: '0 16px 16px'}">
                        <Breadcrumb :style="{margin: '16px 0'}" separator=">">
                            <BreadcrumbItem to="/">工作平台</BreadcrumbItem>
                            <BreadcrumbItem to="工作平台/我的待办">我的待办</BreadcrumbItem>
                        </Breadcrumb>
                        <Card>
                            <div style="height: 900px;">内容区域</div>
                        </Card>
                    </Content>

                </Layout>

            </Layout>

        </Layout>
    </div>

</template>


<script>
    export default {
        
    }
</script>



