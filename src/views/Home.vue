<template>
  <div class="home">
    <mavon-editor v-model="value" @change="change" @save="save" />

    <div @click="save">保存</div>
  </div>
</template>

<script>
export default {
  name: "Home",
  data() {
    return {
      value: "",
    };
  },

  methods: {
    //保存md到后台
    save(value, render) {
      console.log(render);
    },

    change(value, render) {
      // render 为 markdown 解析后的结果
      // console.log(render);
    },
  },
};
</script>
