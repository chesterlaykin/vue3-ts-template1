<template lang="">
<div class="sb-link">
 <RouterLink v-if="buttonData" :to="buttonData.link || ''">
   {{ buttonData.text }}
 </RouterLink>
</div>
</template>
<script lang="ts">
export default {
name: "SBLinkButtonV3",
};
</script>
<script setup lang="ts">
import type { ISBLinkButton } from "@/types/common";
interface IProps {
buttonData?: ISBLinkButton;
bgColor?: string;
}

const props = defineProps<IProps>();

</script>

<style lang="scss">
  //Temporary colors
  $item-bg-color: rgb(77, 129, 234);
  
  .sb-link {
  background: var(--bg-color); //$item-bg-color;
  cursor: pointer;
  font-weight: bold;
  display: inline-block;
  color: rgb(48, 48, 48);
  
  border-radius: 1px;
  border: 1px solid black;
  > a {
   padding-block: 13px;
   padding-inline: 19px;
   display: inline-block;
   color: black;
  }
  &:hover {
   background: rgb(94, 250, 255);
   border: 1px solid rgb(134, 134, 134);
   > a {
     color: $item-bg-color;
   }
   nuxt-link {
     color: rgb(247, 247, 247);
   }
  }
  
  .sb-link-icon {
   width: 14px;
   height: 14px;
   color: red;
   margin-left: 9px;
   fill: purple;
   path {
     fill: rgb(223, 40, 223);
   }
  }
  }
  </style>
  