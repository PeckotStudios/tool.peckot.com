<script setup lang="ts">
import ToolGroup from './components/ToolGroup.vue';
import ToolItem from './components/ToolItem.vue';

</script>

<template>
  <div class="fixed navbar z-10 px-20 min-w-full bg-base-100 backdrop-blur bg-opacity-30">
    <div class="flex-1">
      <a href="https://tool.peckot.com" class="font-extrabold text-lg">Peckot 工具库</a>
    </div>
    <input class="flex-2 input input-bordered w-full max-w-xs" type="text" placeholder="搜索工具…" />
    <div class="flex-none">
      <ul class="menu menu-horizontal px-1">
        <li><a>Link</a></li>
        <li>
          <details>
            <summary>
              Parent
            </summary>
            <ul class="p-2 bg-base-100">
              <li><a>Link 1</a></li>
              <li><a>Link 2</a></li>
            </ul>
          </details>
        </li>
      </ul>
    </div>
  </div>
  <div class="container w-auto mx-32 pt-16 self-center">
    <ToolGroup title="图像工具">
        <ToolItem tool="svg-path-editor" name="SVG Path Editor" desc="在线预览编辑 SVG Path 参数"></ToolItem>
    </ToolGroup>
  </div>
</template>