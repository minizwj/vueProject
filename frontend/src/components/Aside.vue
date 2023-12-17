<template>
      <el-menu :default-openeds="['1']" 
      style="height: 100vh;" 
      :collapse="isCollapse"
      :collapse-transition="false">
      <el-submenu index="1">
        <template slot="title"><i class="el-icon-s-grid"></i>商品管理</template>
        <el-menu-item-group> 
          <el-menu-item index="/addProducts">增加商品信息</el-menu-item>
          <el-menu-item index="/deleteProducts">删除商品信息</el-menu-item>
          <el-menu-item index="/searchProducts">查询商品信息</el-menu-item>
          <el-menu-item index="/editProducts">修改商品信息</el-menu-item>
        </el-menu-item-group>
      </el-submenu>
      <el-submenu index="2">
        <template slot="title"><i class="el-icon-coin"></i>库存管理</template>
        <el-menu-item-group> 
          <el-menu-item index="/searchStore">库存查询</el-menu-item>
          <el-menu-item index="/changeStore">库存调整</el-menu-item>
        </el-menu-item-group>
      </el-submenu>
      <el-submenu index="3">
        <template slot="title"><i class="el-icon-sell"></i>销售管理</template>
        <el-menu-item-group> 
          <el-menu-item index="/sellOrder">销售单</el-menu-item>
          <el-menu-item index="/salesRetrunOrder">退货单</el-menu-item>
          <el-menu-item index="/salesStatistics">销售统计</el-menu-item>
        </el-menu-item-group>
      </el-submenu>
      <el-submenu index="4">
        <template slot="title"><i class="el-icon-s-order"></i>报表管理</template>
        <el-menu-item-group> 
          <el-menu-item index="/salesStatement">商品销售报表</el-menu-item>
          <el-menu-item index="/storeStatement">库存报表</el-menu-item>
          <el-menu-item index="/cashStatement">资金流水报表</el-menu-item>
        </el-menu-item-group>
      </el-submenu>
      <el-submenu index="5">
        <template slot="title"><i class="el-icon-truck"></i>进货管理</template>
        <el-menu-item-group> 
          <el-menu-item index="/purchasePlan">采购计划</el-menu-item>
          <el-menu-item index="/inportOrder">进货单</el-menu-item>
          <el-menu-item index="/suppliers">供货商信息</el-menu-item>
        </el-menu-item-group>
      </el-submenu>
      <el-submenu index="6">
        <template slot="title"><i class="el-icon-s-check"></i>员工管理</template>
        <el-menu-item-group> 
          <el-menu-item index="/employeeProfile">员工资料管理</el-menu-item>
          <el-menu-item index="/authorityManagement">权限分配</el-menu-item>
          <el-menu-item index="/employeeAddentance">员工考勤</el-menu-item>
        </el-menu-item-group>
      </el-submenu>
      
    </el-menu>
</template>

<script>
    export default {
        name: "Aside",
        data(){
          return{
            //isCollapse:false
          }
        },
        props:{
          isCollapse:Boolean
        }
    }
</script>

<style scoped>

</style>