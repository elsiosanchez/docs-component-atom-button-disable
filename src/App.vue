<template>
  <el-card class="box-card">
    <el-card class="box-card">
      <template #header>
        <div class="card-header-attributes">
          <p class="title">
            <b>
              <i>
                {{ "Ejemplo" }}
              </i>
            </b>
          </p>
        </div>
      </template>
      <div style="height: 50px; text-align: center">
        <el-button :disabled="true">
          {{ input }}
        </el-button>
        <el-button :disabled="false">
          {{ input }}
        </el-button>
      </div>
    </el-card>
  </el-card>
</template>

<script lang="ts" setup>
import { ref } from "vue";
const input = ref("Ejemplo");
</script>

<style scoped>
.card-header-attributes {
  text-align: center;
}
.title {
  font-size: 20px;
}
</style>
