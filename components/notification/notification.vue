<template>
    <transition name="fade">
        <div class="notification">
            <span class="content">{{content}}</span>
            <a class="btn" @click="handleClose">{{btn}}</a>
        </div>
    </transition>
</template>
<script>
export default {
    name: 'Notification',
    props: {
        content: {
            type: String,
            required: true
        },
        btn: {
            type: String,
            required: true
        },
    },
    data() {
        return {};
    },
    mounted() {

    },
    methods: {
        handleClose() {

        }
    }
};
</script>
<style scoped>
.notification {
    padding: 15px;
    border-radius: 5px;
    background: #666;
    border: 1px solid rgb(190, 149, 149);
    font-size: 16px;
    width: 250px;
    display: flex;
    text-align: left;
    color: #fff;
}
.content {
    flex: 1;
}
.btn {
    font-size: 12px;
    cursor: pointer;
    color: red;
}
</style>
