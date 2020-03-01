<template>
    <div>
        <el-tree :data="tree" :props="defaultProps" @node-click="handleNodeClick"></el-tree>
    </div>
</template>
<script>
export default {
    name: "DirTree",
    data() {
        return {
            tree: [
                {
                    label: "一级1",
                    id: "1",
                    children: [
                        {
                            label: "二级1-2",
                            id: "1-2"
                        }
                    ]
                },
                {
                    label: "一级2",
                    id: "2",
                    children: [
                        {
                            label: "二级2-2",
                            id: "2-2"
                        }
                    ]
                },
            ],
            defaultProps: {
                children: 'children',
                label: 'label'
            }
        }
    },
    methods: {
        handleNodeClick(data) {
            console.log(data)
        }
    }
}
</script>
<style lang="stylus" scoped>

</style>