<template>
	<div class="home">
		<el-container style="height: 100%">
			<!-- 左边栏 -->
			<el-aside style="border: solid 1px red;">
				<dir-tree></dir-tree>
			</el-aside>
			<!-- 右侧 -->
			<el-container>
				<!-- 头 -->
				<el-header>
					<el-row>
						<el-col :span="12">
							<el-input placeholder="搜索标题/创建人" prefix-icon="el-icon-search"></el-input>
						</el-col>
						<el-col :span="12">
							<span>登陆人信息</span>
						</el-col>
					</el-row>
				</el-header>
				<!-- 主 -->
				<el-main>
					<p>main</p>
				</el-main>
			</el-container>
		</el-container>
	</div>
</template>

<script>
// @ is an alias to /src
import DirTree from "@/components/DirTree.vue";

export default {
	name: "Home",
	components: {
		DirTree
	}
};
</script>
<style scoped>
.home {
	height: 100%;
}
</style>
