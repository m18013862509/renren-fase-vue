<template>
    <div>
        <el-header>
             <!-- 页面头部信息 -->
            <el-input v-model="input" placeholder="表名" style="width:150px;margin-right:10px"></el-input>
            <el-button type="primary" icon="el-icon-search">查询</el-button>
            <el-button type="primary">生成代码</el-button>
        </el-header>
        <!-- 表格 -->
        <el-row>
            <el-table
                :data="tableData"
                border
                style="width: 100%">
                <el-table-column
                prop="date"
                label="日期">
                </el-table-column>
                <el-table-column
                prop="name"
                label="姓名">
                </el-table-column>
                <el-table-column
                prop="address"
                label="地址">
                </el-table-column>
            </el-table>
        </el-row>
    </div>
</template>

<script>
    export default {
        // 过滤器
        filters:{

        },
        // 源数据
        data () {
            return {
                input:'',
                tableData: [{
                    date: '2016-05-03',
                    name: '王小虎',
                    address: '上海市普陀区金沙江路 1518 弄'
                    }, {
                    date: '2016-05-02',
                    name: '王小虎',
                    address: '上海市普陀区金沙江路 1518 弄'
                    }, {
                    date: '2016-05-04',
                    name: '王小虎',
                    address: '上海市普陀区金沙江路 1518 弄'
                    }, {
                    date: '2016-05-01',
                    name: '王小虎',
                    address: '上海市普陀区金沙江路 1518 弄'
                    }, {
                    date: '2016-05-08',
                    name: '王小虎',
                    address: '上海市普陀区金沙江路 1518 弄'
                    }, {
                    date: '2016-05-06',
                    name: '王小虎',
                    address: '上海市普陀区金沙江路 1518 弄'
                    }, {
                    date: '2016-05-07',
                    name: '王小虎',
                    address: '上海市普陀区金沙江路 1518 弄'
                    }]
            }
        },
        // 进入界面就会执行这个方法
        mounted() {
            
        },
        // 普通的方法
        methods: {
            
        },
    }
</script>

<style>

</style>