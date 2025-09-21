<template>
    <div class="d-flex flex-column SlicerContainer">
        <iframe
            src="/klipper-slicer"
            frameborder="0"
            width="100%"
            height="100%"
            allowfullscreen
            webkitallowfullscreen
            mozallowfullscreen>
        </iframe>
    </div>
</template>
<script lang="ts">
import { Component, Mixins } from 'vue-property-decorator'
import BaseMixin from '@/components/mixins/base'

export default class PageSlicer extends Mixins(BaseMixin) {}
</script>


<style scoped>
.SlicerContainer {
    min-height: 400px;
    height: calc(var(--app-height) - 180px);
}
</style>
