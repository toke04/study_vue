<script setup>
import {ref,watch,computed,reactive} from "vue";
const serachWord = ref("")
const names = reactive(
  ["tanaka kouhei",
   "yamaguchi mituo",
   "nakata yasu"
  ])
</script>

<template>
    <div>
        <div class="parent">
          <div>
            <input v-model="serachWord">
              <div>
                <select size="5">
                  <option v-for="name in names">
                      {{ name }}
                  </option>
                </select>
              </div>
          </div>
          <div class="child2">
              <div>
                  <p> <label>名前<input></label></p>
                  <p> <label>苗字<input></label></p>
              </div>
          </div>
        </div>
        <div>
            <button>作成</button>
            <button>更新</button>
            <button>削除</button>
        </div>
    </div>
</template>

<style>
.parent{
    display: flex;
}
.child2{
    margin-left: 20px;
}
</style>
